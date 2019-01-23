---
title: Тип перечисления deviceManagementExchangeAccessStateReason
description: Причина состояния доступа устройства Exchange.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b7a076239e49c59cb95cd1c1f644bc9a2f1f906e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395862"
---
# <a name="devicemanagementexchangeaccessstatereason-enum-type"></a>Тип перечисления deviceManagementExchangeAccessStateReason

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Причина состояния доступа устройства Exchange.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|none|0|Нет причин состояние доступа, обнаруженные в Exchange|
|unknown|1|Причина состояния Неизвестный доступ|
|exchangeGlobalRule|2|Определяет, какие Exchange глобальное правило состояние доступа|
|exchangeIndividualRule|3|Определяет, какие Exchange отдельное правило состояние доступа|
|exchangeDeviceRule|4|Определяет, какие правила устройству Exchange состояние доступа|
|exchangeUpgrade|5|Состояние доступа из-за обновления Exchange|
|exchangeMailboxPolicy|6|Состояние доступа определяет, какие политики почтовых ящиков Exchange|
|другие|7|Определяет, какие Exchange состояние доступа|
|спецификации|8|Состояние доступа, предоставленных с соответствием требованиям сложности при реализации|
|notCompliant|9|Состояние доступа отозван соответствия требованиям сложности при реализации|
|notEnrolled|10|Состояние доступа отозван сложности при реализации управления|
|unknownLocation|12|Состояние доступа из-за неизвестное расположение|
|mfaRequired|13|Состояние доступа из-за сложности при реализации многофакторной проверкой Подлинности|
|azureADBlockDueToAccessPolicy|14|Состояние доступа отозван политикой доступа AAD|
|compromisedPassword|15|Состояние доступа отозван компрометации пароля|
|deviceNotKnownWithManagedApp|16|Состояние доступа отозван запрос управляемых приложений|




