---
title: Отчеты о действиях пользователей Microsoft Teams
description: С помощью отчетов о действиях пользователей Microsoft Teams можно анализировать действия пользователей Microsoft Teams в организации.
ms.localizationpriority: high
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: a2c61edbc5e8df05fb47eca2f34dfb2b84606c9b
ms.sourcegitcommit: 69b150e408c0b9a0705bf33229269f6e5371bc6c
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/07/2022
ms.locfileid: "65923969"
---
# <a name="microsoft-teams-user-activity-reports"></a>Отчеты о действиях пользователей Microsoft Teams

Пространство имен: microsoft.graph

С помощью отчетов о действиях пользователей Microsoft Teams можно анализировать действия пользователей Microsoft Teams в организации.

## <a name="methods"></a>Методы

| Метод                                   | Возвращаемый тип | Описание                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [Получение сведений о пользователях](../api/reportroot-getteamsuseractivityuserdetail.md) | Stream      | Получение сведения о действиях отдельных пользователей Microsoft Teams. |
| [Получение количества действий](../api/reportroot-getteamsuseractivitycounts.md) | Stream      | Получение количества действий Microsoft Teams по типам. Действия выполняют лицензированные пользователи Microsoft Teams. |
| [Получение количества пользователей](../api/reportroot-getteamsuseractivityusercounts.md) | Stream      | Получение сведений о количестве пользователей по типам действий. К типам действий относятся сообщения в чатах групп, сообщения в частных чатах, звонки и собрания. |

