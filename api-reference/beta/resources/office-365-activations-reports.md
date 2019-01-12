---
title: Отчеты об активации Office 365
description: Отчет активации Office 365 позволяет представление, из которых пользователи активации Office 365 подписок на по крайней мере одно устройство. Предоставляет декомпозиции Office 365 ProPlus, Project и Visio Pro для активации подписки Office 365, а также декомпозиции активаций различных рабочего стола и устройств. В этом отчете может помочь определить пользователей, которые могут потребоваться дополнительную поддержку для активации подписки Office.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 8f9c174ba1439825ff08edb33518da74f6a77634
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27978622"
---
# <a name="office-365-activations-reports"></a>Отчеты об активации Office 365

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Отчет активации Office 365 позволяет представление, из которых пользователи активации Office 365 подписок на по крайней мере одно устройство. Предоставляет декомпозиции Office 365 ProPlus, Project и Visio Pro для активации подписки Office 365, а также декомпозиции активаций различных рабочего стола и устройств. В этом отчете может помочь определить пользователей, которые могут потребоваться дополнительную поддержку для активации подписки Office.

> **Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).

## <a name="reports"></a>Отчеты
| Функция                                 | Возвращаемый тип CSV | Возвращаемый тип JSON                         | Описание                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Получение сведений о пользователях](../api/reportroot-getoffice365activationsuserdetail.md) | Stream          | [office365ActivationsUserDetail](../resources/office365activationsuserdetail.md) | Получите сведения о пользователях, которые активировали Office 365. |
| [Получение количества активаций](../api/reportroot-getoffice365activationcounts.md) | Поток          | [office365ActivationCounts](../resources/office365activationcounts.md) | Получите сведения о количестве активаций Office 365 на компьютерах и мобильных устройствах. |
| [Получение количества пользователей](../api/reportroot-getoffice365activationsusercounts.md) | Stream          | [office365ActivationsUserCounts](../resources/office365activationsusercounts.md) | Узнайте, сколько пользователей активировали подписку на Office на компьютере или мобильном устройстве. |
