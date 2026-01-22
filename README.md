// SPDX-License-Identifier: MIT
pragma solidity ^0.8.20;

/// @title IStrategy
/// @notice Defines a generic interface for DeFi automation strategies
/// @dev All strategies must be non-custodial and parameter constrained
interface IStrategy {
    /// @notice Execute a strategy action
    /// @param data Encoded parameters defining execution constraints
    function execute(bytes calldata data) external;

    /// @notice Validate strategy parameters before execution
    /// @param data Encoded parameters
    /// @return valid True if parameters are valid
    function validate(bytes calldata data) external view returns (bool valid);
}
## Project Structure

- contracts/
  - core/ — core execution engine
  - adapters/ — protocol integrations
  - permissions/ — DAO permission control
  - interfaces/ — shared interfaces
- test/ — unit tests
- scripts/ — deployment/testing scripts
- docs/ — additional documentation# RIYP Money Tree Bot

Ethereum-native DeFi automation infrastructure for non-custodial execution of lending, yield, and treasury strategies.

This repository contains smart contract scaffolding, security documentation, and milestone planning for ecosystem grant evaluation.
