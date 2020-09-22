---
title: Отчеты об активации Microsoft 365
description: Отчет об активации Microsoft 365 предоставляет представление о том, какие пользователи активировали подписки Microsoft 365 по крайней мере на одном устройстве. Он содержит сведения об активации Microsoft 365 профессиональный плюс, Project и Visio Pro для активации подписки Microsoft 365, а также разделение активаций на настольных компьютерах и устройствах. Этот отчет поможет определить пользователей, которым может потребоваться дополнительная поддержка для активации подписки на Office.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 86a418e75fee70d16009f0ab6f8a3f0f474760cd
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021261"
---
# <a name="microsoft-365-activations-reports"></a>Отчеты об активации Microsoft 365

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Отчет об активации Microsoft 365 предоставляет представление о том, какие пользователи активировали подписки Microsoft 365 по крайней мере на одном устройстве. Он содержит сведения об активации Microsoft 365 профессиональный плюс, Project и Visio Pro для активации подписки Microsoft 365, а также разделение активаций на настольных компьютерах и устройствах. Этот отчет поможет определить пользователей, которым может потребоваться дополнительная поддержка для активации подписки на Office.

> **Примечание:** Сведения о различных представлениях отчетов и их именах можно найти в [статье Microsoft 365 Reports — активации Microsoft Office](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).

## <a name="reports"></a>Отчеты
| Функция                                 | Возвращаемый тип CSV | Возвращаемый тип JSON                         | Описание                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Получение сведений о пользователях](../api/reportroot-getoffice365activationsuserdetail.md) | Stream          | [office365ActivationsUserDetail](../resources/office365activationsuserdetail.md) | Получение сведений о пользователях, которые активировали Microsoft 365. |
| [Получение количества активаций](../api/reportroot-getoffice365activationcounts.md) | Поток          | [office365ActivationCounts](../resources/office365activationcounts.md) | Получение числа активаций Microsoft 365 на настольных компьютерах и устройствах. |
| [Получение количества пользователей](../api/reportroot-getoffice365activationsusercounts.md) | Stream          | [office365ActivationsUserCounts](../resources/office365activationsusercounts.md) | Узнайте, сколько пользователей активировали подписку на Office на компьютере или мобильном устройстве. |


