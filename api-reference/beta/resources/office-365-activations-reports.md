---
title: Microsoft 365 отчеты об активациях
description: Отчет Microsoft 365 активации позволяет просмотреть, какие пользователи активировали Microsoft 365 по крайней мере на одном устройстве. В нем содержится разбивка Microsoft 365 ProPlus, Project и Visio Pro для Microsoft 365 активаций подписки, а также разбивка активаций на настольных компьютерах и устройствах. В этом отчете можно определить пользователей, которым может потребоваться дополнительная поддержка для активации Office подписки.
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: ca3a0218b288105982cb67664629a467a67d596a
ms.sourcegitcommit: f336c5c49fbcebe55312656aa8b50511fd99a657
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/09/2021
ms.locfileid: "61390629"
---
# <a name="microsoft-365-activations-reports"></a>Microsoft 365 отчеты об активациях

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Отчет Microsoft 365 активации позволяет просмотреть, какие пользователи активировали Microsoft 365 по крайней мере на одном устройстве. В нем содержится разбивка Microsoft 365 ProPlus, Project и Visio Pro для Microsoft 365 активаций подписки, а также разбивка активаций на настольных компьютерах и устройствах. В этом отчете можно определить пользователей, которым может потребоваться дополнительная поддержка для активации Office подписки.

> **Примечание:** Сведения о различных представлениях отчетов и [именах см. в Microsoft 365 отчетов — Microsoft Office активаций.](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60)

## <a name="reports"></a>Отчеты
| Функция                                                     | Тип возврата CSV | Тип возврата JSON | Описание                                                  |
| :----------------------------------------------------------- | :-------------- | :--------------- | ------------------------------------------------------------ |
| [Получение сведений о пользователях](../api/reportroot-getoffice365activationsuserdetail.md) | Stream          | Stream           | Сведения о пользователях, активировавших Microsoft 365.    |
| [Получение количества активаций](../api/reportroot-getoffice365activationcounts.md) | Поток          | Stream           | Получите количество активаций Microsoft 365 на настольных компьютерах и устройствах. |
| [Получение количества пользователей](../api/reportroot-getoffice365activationsusercounts.md) | Stream          | Поток           | Узнайте, сколько пользователей активировали подписку на Office на компьютере или мобильном устройстве. |


