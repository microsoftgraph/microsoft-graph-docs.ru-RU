---
title: Отчеты об активациях Microsoft 365
description: Отчет об активации Microsoft 365 позволяет просмотреть, какие пользователи активировали подписки Microsoft 365 хотя бы на одном устройстве. Он предоставляет разбивку по активациям подписок Microsoft 365 профессиональныйplus, Project и Visio Pro для Microsoft 365, а также разбивку активаций на настольных компьютерах и устройствах. Этот отчет поможет определить пользователей, которым может потребоваться дополнительная поддержка для активации их подписки на Office.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 32fb2f1397218a5d6c99b071b7a398cf00cd54f7
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49980803"
---
# <a name="microsoft-365-activations-reports"></a>Отчеты об активациях Microsoft 365

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Отчет об активации Microsoft 365 позволяет просмотреть, какие пользователи активировали подписки Microsoft 365 хотя бы на одном устройстве. Он предоставляет разбивку по активациям подписок Microsoft 365 профессиональныйplus, Project и Visio Pro для Microsoft 365, а также разбивку активаций на настольных компьютерах и устройствах. Этот отчет поможет определить пользователей, которым может потребоваться дополнительная поддержка для активации подписки на Office.

> **Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в отчетах [Microsoft 365 Microsoft Office активации.](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60)

## <a name="reports"></a>Отчеты
| Функция                                 | Тип возврата CSV | Тип возврата JSON                         | Описание                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Получение сведений о пользователях](../api/reportroot-getoffice365activationsuserdetail.md) | Stream          | [office365ActivationsUserDetail](../resources/office365activationsuserdetail.md) | Получите сведения о пользователях, активировавших Microsoft 365. |
| [Получение количества активаций](../api/reportroot-getoffice365activationcounts.md) | Поток          | [office365ActivationCounts](../resources/office365activationcounts.md) | Получите количество активаций Microsoft 365 на настольных компьютерах и устройствах. |
| [Получение количества пользователей](../api/reportroot-getoffice365activationsusercounts.md) | Stream          | [office365ActivationsUserCounts](../resources/office365activationsusercounts.md) | Узнайте, сколько пользователей активировали подписку на Office на компьютере или мобильном устройстве. |


