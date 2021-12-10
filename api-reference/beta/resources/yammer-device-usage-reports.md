---
title: Отчеты об использовании устройств с Yammer
description: Отчеты об использовании устройств с Yammer содержат сведения о том, какие устройства с Yammer есть у пользователей. Вы можете просматривать сведения о количестве пользователей за указанный период с разбивкой по типам устройств и по пользователям.
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: b9d5a7d2ea6cd8e02e26414618b27acf441444cd
ms.sourcegitcommit: f336c5c49fbcebe55312656aa8b50511fd99a657
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/09/2021
ms.locfileid: "61390055"
---
# <a name="yammer-device-usage-reports"></a>Отчеты об использовании устройств с Yammer

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Отчеты об использовании устройств с Yammer содержат сведения о том, какие устройства с Yammer есть у пользователей. Вы можете просматривать сведения о количестве пользователей за указанный период с разбивкой по типам устройств и по пользователям.

> **Примечание:** Подробные сведения о различных представлениях отчетов и [именах см. в Microsoft 365 отчетов - Yammer устройства.](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38)

## <a name="reports"></a>Отчеты

| Функция                                                     | Тип возврата CSV | Тип возврата JSON | Описание                                    |
| :----------------------------------------------------------- | :-------------- | :--------------- | ---------------------------------------------- |
| [Получение сведений о пользователях](../api/reportroot-getyammerdeviceusageuserdetail.md) | Stream          | Stream           | Получение сведений об использовании устройств с Yammer с разбивкой по пользователям. |
| [Получение количества пользователей с разбивкой по устройствам](../api/reportroot-getyammerdeviceusagedistributionusercounts.md) | Stream          | Stream           | Получение сведений о количестве пользователей с разбивкой по типам устройств.        |
| [Получение количества пользователей](../api/reportroot-getyammerdeviceusageusercounts.md) | Stream          | Stream           | Получение сведений о количестве пользователей в день с разбивкой по типам устройств.  |


