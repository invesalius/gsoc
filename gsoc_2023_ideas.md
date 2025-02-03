#This is a sample code for Logging and error control Python has a module logging which can be used for this. 

import logging

def setup_logging():
    # Create a logger
    logger = logging.getLogger('my_logger')
    logger.setLevel(logging.DEBUG)

    # Create file handler which logs all messages
    file_handler = logging.FileHandler('event_log.txt')
    file_handler.setLevel(logging.DEBUG)

    # Create a formatter and add it to the handler
    formatter = logging.Formatter('%(asctime)s - %(levelname)s - %(message)s')
    file_handler.setFormatter(formatter)

    # Add the handler to the logger
    logger.addHandler(file_handler)

    return logger

# Example usage
if __name__ == "__main__":
    # Setup logging
    logger = setup_logging()

    # Log some events
    logger.debug('Debug message')
    logger.info('Informational message')
    logger.warning('Warning message')
    logger.error('Error message')
    logger.critical('Critical error message')
