---
title: Microsoft Teams отчеты об использовании команды
description: Используйте отчеты Microsoft Teams использования команд, чтобы получить представление об использовании команд в организации.
ms.localizationpriority: medium
ms.prod: reports
author: zhiliqiao
doc_type: conceptualPageType
ms.openlocfilehash: df580adb2234902cf9093714fd4e627f67581491
ms.sourcegitcommit: 9bbcce5784a89768ece55a66e3651080d56e1e92
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/19/2022
ms.locfileid: "64917964"
---
# <a name="microsoft-teams-team-usage-reports"></a>Microsoft Teams отчеты об использовании команды

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используйте отчеты Microsoft Teams использования команд, чтобы получить представление об использовании команд в организации.

## <a name="reports"></a>Отчеты

| Функция | Тип возвращаемого CSV-файла | Тип возвращаемого значения JSON | Описание |
| :--------------------------------------- | --------------- | ---------------------------------------- | ---------------------------------------- |
| [Получение сведений о команде](../api/reportroot-getteamsteamactivitydetail.md) | Stream | Stream | Получение сведений о Teams действий по командам. Эти числа включают действия как для лицензированных, так и для пользователей без лицензии. |
| [Получение количества команд](../api/reportroot-getteamsteamactivitycounts.md) | Stream | Stream | Получение количества командных действий в Microsoft Teams. Типы действий связаны с собраниями и сообщениями. |
| [Получение количества групп рассылки](../api/reportroot-getteamsteamactivitydistributioncounts.md) | Stream | Stream | Получение количества действий команды в Microsoft Teams за выбранный период. |


