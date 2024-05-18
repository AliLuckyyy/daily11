# daily11
pragma solidity ^0.8.0;

contract DailyCalendar {
    mapping(uint256 => string) public events;

    function addEvent(uint256 date, string memory eventDescription) public {
        events[date] = eventDescription;
    }

    function getEvent(uint256 date) public view returns (string memory) {
        return events[date];
    }
}
