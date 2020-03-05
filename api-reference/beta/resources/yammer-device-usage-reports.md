---
title: Отчеты об использовании устройств с Yammer
description: Отчеты об использовании устройств с Yammer содержат сведения о том, какие устройства с Yammer есть у пользователей. Вы можете просматривать сведения о количестве пользователей за указанный период с разбивкой по типам устройств и по пользователям.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 02d5f3bcb71b343b0406536d77d80d477cc71223
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519052"
---
# <a name="yammer-device-usage-reports"></a>Отчеты об использовании устройств с Yammer

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Отчеты об использовании устройств с Yammer содержат сведения о том, какие устройства с Yammer есть у пользователей. Вы можете просматривать сведения о количестве пользователей за указанный период с разбивкой по типам устройств и по пользователям.

> **Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: использование устройств с Yammer](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).

## <a name="reports"></a>Отчеты

| Функция                                 | Возвращаемый тип CSV | Возвращаемый тип JSON                         | Описание                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Получение сведений о пользователях](../api/reportroot-getyammerdeviceusageuserdetail.md) | Поток          | [яммердевицеусажеусердетаил](../resources/yammerdeviceusageuserdetail.md) | Получение сведений об использовании устройств с Yammer с разбивкой по пользователям. |
| [Получение количества пользователей с разбивкой по устройствам](../api/reportroot-getyammerdeviceusagedistributionusercounts.md) | Stream          | [яммердевицеусажедистрибутионусеркаунтс](../resources/yammerdeviceusagedistributionusercounts.md) | Получение сведений о количестве пользователей с разбивкой по типам устройств.  |
| [Получение количества пользователей](../api/reportroot-getyammerdeviceusageusercounts.md) | Stream          | [яммердевицеусажеусеркаунтс](../resources/yammerdeviceusageusercounts.md) | Получение сведений о количестве пользователей в день с разбивкой по типам устройств. |
