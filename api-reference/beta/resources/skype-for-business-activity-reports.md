---
title: Отчеты о работе со Skype для бизнеса
description: Сведения о действиях можно получить в организации. Эти данные могут пригодиться при проведении анализа, планировании и принятии других бизнес-решений.
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: cdf87a582b231548af829def11e6a182d6ce5ba0
ms.sourcegitcommit: f336c5c49fbcebe55312656aa8b50511fd99a657
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/09/2021
ms.locfileid: "61390929"
---
# <a name="skype-for-business-activity-reports"></a>Отчеты о работе со Skype для бизнеса

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Сведения о действиях можно получить в организации. Эти данные могут пригодиться при проведении анализа, планировании и принятии других бизнес-решений.

> **Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Microsoft 365: действия в Skype для бизнеса](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).

## <a name="reports"></a>Отчеты

| Функция                                                     | Тип возврата CSV | Тип возврата JSON | Описание                                                  |
| :----------------------------------------------------------- | :-------------- | :--------------- | ------------------------------------------------------------ |
| [Получение сведений о пользователях](../api/reportroot-getskypeforbusinessactivityuserdetail.md) | Stream          | Поток           | Получите сведения о действиях пользователей в Skype для бизнеса.       |
| [Получение количества действий](../api/reportroot-getskypeforbusinessactivitycounts.md) | Stream          | Stream           | Отслеживайте, как меняется количество организаторов и участников конференций, проводимых в вашей организации через Skype для бизнеса. Отчет также включает количество одноранговых сеансов. |
| [Получение количества пользователей](../api/reportroot-getskypeforbusinessactivityusercounts.md) | Stream          | Stream           | Отслеживайте, как меняется количество уникальных организаторов и участников конференций, проводимых в вашей организации через Skype для бизнеса. Отчет также включает количество одноранговых сеансов. |


