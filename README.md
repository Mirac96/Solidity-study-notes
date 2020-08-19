# Solidity-study-notes
the notes during studying solidity

View and pure:
Starting with solc 0.4.17, constant is depricated in favor of two new and more specific modifiers.
View This is generally the replacement for constant. It indicates that the function will not alter the storage state in any way.
Pure This is even more restrictive, indicating that it won't even read the storage state.
A pure function might look something like this very contrived example:

function returnTrue() public pure returns(bool response) {
    return true;
}
