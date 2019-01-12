---
title: Тип перечисления deviceManagementExchangeAccessStateReason
description: Причина состояния доступа устройства Exchange.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 25d5ac8a5624352b9c474caf4088709ca1453387
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981849"
---
# <a name="devicemanagementexchangeaccessstatereason-enum-type"></a>Тип перечисления deviceManagementExchangeAccessStateReason

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Причина состояния доступа устройства Exchange.
## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|Нет|0|Нет причин состояние доступа, обнаруженные в Exchange|
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





