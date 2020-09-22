---
title: Отчеты об использовании устройств с Yammer
description: Отчеты об использовании устройств с Yammer содержат сведения о том, какие устройства с Yammer есть у пользователей. Вы можете просматривать сведения о количестве пользователей за указанный период с разбивкой по типам устройств и по пользователям.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: c23e67c22189ff08468b44b1993034616dd74e27
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48070417"
---
# <a name="yammer-device-usage-reports"></a>Отчеты об использовании устройств с Yammer

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Отчеты об использовании устройств с Yammer содержат сведения о том, какие устройства с Yammer есть у пользователей. Вы можете просматривать сведения о количестве пользователей за указанный период с разбивкой по типам устройств и по пользователям.

> **Примечание:** Сведения о различных представлениях отчетов и их именах можно найти в [статье Microsoft 365 Reports-Device Device Usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).

## <a name="reports"></a>Отчеты

| Функция                                 | Возвращаемый тип CSV | Возвращаемый тип JSON                         | Описание                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Получение сведений о пользователях](../api/reportroot-getyammerdeviceusageuserdetail.md) | Stream          | [яммердевицеусажеусердетаил](../resources/yammerdeviceusageuserdetail.md) | Получение сведений об использовании устройств с Yammer с разбивкой по пользователям. |
| [Получение количества пользователей с разбивкой по устройствам](../api/reportroot-getyammerdeviceusagedistributionusercounts.md) | Stream          | [яммердевицеусажедистрибутионусеркаунтс](../resources/yammerdeviceusagedistributionusercounts.md) | Получение сведений о количестве пользователей с разбивкой по типам устройств.  |
| [Получение количества пользователей](../api/reportroot-getyammerdeviceusageusercounts.md) | Stream          | [яммердевицеусажеусеркаунтс](../resources/yammerdeviceusageusercounts.md) | Получение сведений о количестве пользователей в день с разбивкой по типам устройств. |


