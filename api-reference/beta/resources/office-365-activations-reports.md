---
title: Отчеты об активации Office 365
description: Отчет активации Office 365 позволяет представление, из которых пользователи активации Office 365 подписок на по крайней мере одно устройство. Предоставляет декомпозиции Office 365 ProPlus, Project и Visio Pro для активации подписки Office 365, а также декомпозиции активаций различных рабочего стола и устройств. В этом отчете может помочь определить пользователей, которые могут потребоваться дополнительную поддержку для активации подписки Office.
ms.openlocfilehash: 745ca24de47f576522f2f81e3f9d7b70921d81ea
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081442"
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
