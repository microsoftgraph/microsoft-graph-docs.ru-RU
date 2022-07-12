---
title: Тип перечисления deviceManagementExchangeAccessStateReason
description: Причина состояния доступа к Обмену устройствами.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: f6cc10fd962a43ed87179299f22e48d84c7c13ba
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/12/2022
ms.locfileid: "66736071"
---
# <a name="devicemanagementexchangeaccessstatereason-enum-type"></a>Тип перечисления deviceManagementExchangeAccessStateReason

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Причина состояния доступа к Обмену устройствами.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|none|0|Причина состояния доступа не обнаружена в Exchange|
|unknown|1|Неизвестная причина состояния доступа|
|exchangeGlobalRule|2|Состояние доступа, определяемого глобальным правилом Exchange|
|exchangeIndividualRule|3|Состояние доступа, определяемого правилом Exchange Individual|
|exchangeDeviceRule|4|Состояние доступа, определяемого правилом устройства Exchange|
|ExchangeUpgrade|5|Состояние доступа из-за обновления Exchange|
|exchangeMailboxPolicy|6 |Состояние доступа, определяемая политикой почтовых ящиков Exchange|
|Других|7 |Состояние доступа, определяемого Exchange|
|Совместимый|8 |Состояние доступа, предоставленное запросом на соответствие требованиям|
|notCompliant|9 |Состояние доступа, отозванное в соответствии с запросом на соответствие|
|notEnrolled|10|Состояние доступа, отозванное задачей управления|
|unknownLocation|12 |Состояние доступа из-за неизвестного расположения|
|mfaRequired|13|Состояние доступа из-за запроса MFA|
|azureADBlockDueToAccessPolicy|14|Состояние доступа, отозванное политикой доступа AAD|
|compromisedPassword|15|Состояние доступа, отозванное скомпрометированным паролем|
|deviceNotKnownWithManagedApp|16|Состояние доступа, отозванное задачей управляемого приложения|





