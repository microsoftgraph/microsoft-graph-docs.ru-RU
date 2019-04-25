---
title: Проверки доступа Azure AD
description: Вы можете использовать обзоры Azure AD, чтобы настроить однократные или повторяющиеся проверки доступа для подтверждения прав доступа пользователя.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 212af4ad8519f7ec54fb56ceffee0a0d4de16027
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32544136"
---
# <a name="azure-ad-access-reviews"></a>Проверки доступа Azure AD

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Вы можете использовать [обзоры Azure AD](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-azure-ad-controls-access-reviews-overview) , чтобы настроить однократные или повторяющиеся проверки доступа для подтверждения прав доступа пользователя.

Типичные сценарии клиентов для проверки членства в группах и доступа к приложениям:
   
- Пользователи могут просматривать и сертифицировать гостевой доступ, используя обзоры доступа к приложениям и группам. Проверяющие могут использовать аналитику, которая позволяет эффективно определять, должен ли гостям доступ.
      
- Пользователи могут просматривать и сертифицировать доступ сотрудников к приложениям и членству в группах с помощью рецензирования Access.
   
- Пользователи могут собирать элементы управления проверкой доступа в программы, которые соответствуют требованиям организации для отслеживания проверок на соответствие требованиям и приложениям, учитывающим риск.

Кроме того, у пользователей есть возможность просматривать и сертифицировать назначения ролей для пользователей, которым назначены роли Azure AD, такие как глобальный администратор или роли подписки Azure.  Эта возможность включена в [Azure AD с правами привилегированНого управления идентификацией](privilegedidentitymanagement-root.md).

Обратите внимание, что функция рецензирования доступа, включая API, включена в Azure AD Premium P2. 

## <a name="methods"></a>Методы

Ниже приведен список методов, предоставляемых проверками доступа Azure AD.  

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение Акцессревиев](../api/accessreview-get.md) |   [Акцессревиев](accessreview.md) |   Получение проверки доступа с определенным идентификатором. |
|[Создание Акцессревиев](../api/accessreview-create.md) | [Акцессревиев](accessreview.md) |   Создание нового Акцессревиев. |
|[Удаление Акцессревиев](../api/accessreview-delete.md) | Нет.   | Удаление Акцессревиев. |
|[Обновление Акцессревиев](../api/accessreview-update.md) | [Акцессревиев](accessreview.md) | Обновление Акцессревиев. |
|[Список рецензентов Акцессревиев](../api/accessreview-listreviewers.md) |      Коллекция [userIdentity](useridentity.md)| Получение рецензентов объекта Акцессревиев. |
|[Добавление рецензента Акцессревиев](../api/accessreview-addreviewer.md) |      Нет.   |   Добавьте проверяющего в объект Акцессревиев. |
|[Удаление рецензента Акцессревиев](../api/accessreview-removereviewer.md) | Нет.  |   Удаление проверяющего из Акцессревиев. |
|[Список решений Акцессревиев](../api/accessreview-listdecisions.md) |      Коллекция [акцессревиевдеЦисион](accessreviewdecision.md)| Получение решений для Акцессревиев.|
|[Список моих решений Акцессревиев](../api/accessreview-listmydecisions.md) |     Коллекция [акцессревиевдеЦисион](accessreviewdecision.md)| В качестве проверяющего получите мое решение Акцессревиев.|
|[Отправка напоминания о Акцессревиев](../api/accessreview-sendreminder.md) |        Нет.   |   Отправьте напоминание рецензентам Акцессревиев. |
|[Остановить Акцессревиев](../api/accessreview-stop.md) |     Нет.   |   Остановка Акцессревиев. |
|[Сброс решений Акцессревиев](../api/accessreview-reset.md) |     Нет.   |   Сброс решений во время выполнения Акцессревиев.|
|[Применение решений Акцессревиев](../api/accessreview-apply.md) |     Нет.   |   Применение решений из завершенной Акцессревиев.|
|[Список Бусинессфловтемплатес](../api/businessflowtemplate-list.md) | Коллекция [бусинессфловтемплате](businessflowtemplate.md)| Получите шаблоны бизнес-процесса, подходящие для доступа к рецензированию.|
|[Создание программы](../api/program-create.md) |   [Программа](program.md)   |   Создайте новую программу.|
|[Удаление программы](../api/program-delete.md) |   Нет.   |   Удаление программы.|
|[Список программ](../api/program-list.md) |  Коллекция [Program](program.md)|   Получение коллекции всех программ.|
|[Список Програмконтролс программы](../api/program-listcontrols.md) |      Коллекция [програмконтрол](programcontrol.md)| Получение коллекции элементов управления программы.|
|[Программа обновления](../api/program-update.md) |   [Программа](program.md)|  Обновление программы.|
|[Создание Програмконтрол](../api/programcontrol-create.md) |     [Програмконтрол](programcontrol.md) |   Добавление Програмконтрол в программу.|
|[Удаление Програмконтрол](../api/programcontrol-delete.md) |     Нет.   |   Удаление Програмконтрол из программы.|
|[Список Програмконтролс](../api/programcontrol-list.md) | Коллекция [програмконтрол](programcontrol.md)| ПереЧисление элементов управления для всех программ в клиенте.|
|[Список Програмконтролтипес](../api/programcontroltype-list.md) | Коллекция [програмконтролтипе](programcontroltype.md)| Список типов элементов управления программы. |


## <a name="see-also"></a>См. также

- [Как администратор может управлять доступом пользователей с помощью проверок доступа Azure AD](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-azure-ad-controls-manage-user-access-with-access-reviews)
- [Как администратор может управлять гостевым доступом с помощью проверок Azure AD](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-azure-ad-controls-manage-guest-access-with-access-reviews)
- [Как администратор может управлять программами и элементами управления для рецензирования Access Azure AD](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-azure-ad-controls-manage-programs-controls)


<!--
{
  "type": "#page.annotation",
  "description": "Service root",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/accessreviews-root.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
