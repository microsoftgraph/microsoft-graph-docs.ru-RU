---
title: тип enum deviceManagementExchangeAccessStateReason
description: Причина Exchange доступа к состоянию устройства.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 5f6b1dd60e9a8880502bd04e77efc3a0dc53f82b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59125983"
---
# <a name="devicemanagementexchangeaccessstatereason-enum-type"></a>тип enum deviceManagementExchangeAccessStateReason

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Причина Exchange доступа к состоянию устройства.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|Нет|0|Причина состояния доступа, обнаруженная в Exchange|
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
|compromisedPassword|15 |Состояние доступа отозвано с помощью скомпрометированного пароля|
|deviceNotKnownWithManagedApp|16 |Доступ к состояниям, отозванным из-за проблемы управляемого приложения|



