---
title: тип enum deviceManagementExchangeAccessStateReason
description: Причина Exchange доступа к состоянию устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 7aa61e8ecdf88663123a486cb9bccb033aeecbb5
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754576"
---
# <a name="devicemanagementexchangeaccessstatereason-enum-type"></a>тип enum deviceManagementExchangeAccessStateReason

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Причина Exchange доступа к состоянию устройства.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|нет|0|Причина состояния доступа, обнаруженная в Exchange|
|unknown|1|Причина состояния неизвестного доступа|
|exchangeGlobalRule|2|Состояние доступа, Exchange глобальное правило|
|exchangeIndividualRule|3|Состояние доступа, определяемая Exchange индивидуальным правилом|
|exchangeDeviceRule|4 |Состояние доступа, определяющееся Exchange устройства|
|exchangeUpgrade|5 |Состояние доступа из-за Exchange обновления|
|exchangeMailboxPolicy|6 |Состояние доступа, определяемого политикой Exchange почтовых ящиков|
|другие|7 |Состояние доступа, определяемая Exchange|
|совместимый|8 |Состояние доступа, предоставленная проблемой соответствия требованиям|
|notCompliant|9 |Доступ к состояниям, отозванным из-за проблемы соответствия требованиям|
|notEnrolled|10 |Доступ к состояниям, отозванным из-за проблемы управления|
|unknownLocation|12 |Состояние доступа из-за неизвестного расположения|
|mfaRequired|13|Состояние доступа из-за проблемы с MFA|
|azureADBlockDueToAccessPolicy|14 |Состояние доступа отозвано политикой доступа AAD|
|compromisedPassword|15|Состояние доступа отозвано с помощью скомпрометированного пароля|
|deviceNotKnownWithManagedApp|16 |Доступ к состояниям, отозванным из-за проблемы управляемого приложения|




