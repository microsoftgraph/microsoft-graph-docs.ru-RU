---
title: Отчеты об активации Office 365
description: Отчет об активации Office 365 предоставляет представление о том, какие пользователи активировали подписки на Office 365 по крайней мере на одном устройстве. Он содержит сведения об активации подписки на Office 365 профессиональный плюс, Project и Visio Pro для Office 365, а также разделение активаций на настольных компьютерах и устройствах. Этот отчет поможет определить пользователей, которым может потребоваться дополнительная поддержка для активации подписки на Office.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 7b72245efc971be468ae050c387c6be3665c013a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522514"
---
# <a name="office-365-activations-reports"></a>Отчеты об активации Office 365

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Отчет об активации Office 365 предоставляет представление о том, какие пользователи активировали подписки на Office 365 по крайней мере на одном устройстве. Он содержит сведения об активации подписки на Office 365 профессиональный плюс, Project и Visio Pro для Office 365, а также разделение активаций на настольных компьютерах и устройствах. Этот отчет поможет определить пользователей, которым может потребоваться дополнительная поддержка для активации подписки на Office.

> **Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).

## <a name="reports"></a>Отчеты
| Функция                                 | Возвращаемый тип CSV | Возвращаемый тип JSON                         | Описание                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Получение сведений о пользователях](../api/reportroot-getoffice365activationsuserdetail.md) | Stream          | [office365ActivationsUserDetail](../resources/office365activationsuserdetail.md) | Получите сведения о пользователях, которые активировали Office 365. |
| [Получение количества активаций](../api/reportroot-getoffice365activationcounts.md) | Поток          | [office365ActivationCounts](../resources/office365activationcounts.md) | Получите сведения о количестве активаций Office 365 на компьютерах и мобильных устройствах. |
| [Получение количества пользователей](../api/reportroot-getoffice365activationsusercounts.md) | Stream          | [office365ActivationsUserCounts](../resources/office365activationsusercounts.md) | Узнайте, сколько пользователей активировали подписку на Office на компьютере или мобильном устройстве. |
