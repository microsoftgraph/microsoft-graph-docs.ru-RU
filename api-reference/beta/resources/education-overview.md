---
title: Работа с интерфейсами API для образования в Microsoft Graph
description: Интерфейсы API в Microsoft Graph education Улучшите ресурсов Office 365 и данных с помощью сведений, имеющих отношение к education сценарии, включая школ, студентов, преподавателей, классы, регистрации и назначений. Это упрощает создание решений, интегрируемых с образовательными ресурсами.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 9e106da7eb717a091941e16f4a70af8a012802f3
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516933"
---
# <a name="working-with-education-apis-in-microsoft-graph"></a>Работа с интерфейсами API для образования в Microsoft Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Интерфейсы API в Microsoft Graph education Улучшите ресурсов Office 365 и данных с помощью сведений, имеющих отношение к education сценарии, включая школ, студентов, преподавателей, классы, регистрации и назначений. Это упрощает создание решений, интегрируемых с образовательными ресурсами.

Образование API-интерфейсы включают rostering ресурсов и назначений, которые можно использовать для взаимодействия со службами rostering и назначений в группах Майкрософт. Эти ресурсы можно использовать для управления школа участников и автоматизации учащихся.

## <a name="authorization"></a>Авторизация

Чтобы вызывать API для образования в Microsoft Graph, приложению необходимо получить маркер доступа. Подробные сведения о маркерах доступа см. в статье [Получение маркеров доступа для вызова Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview). Приложению также потребуются соответствующие разрешения. Дополнительные сведения см. в разделе [Разрешения для образования](/graph/permissions-reference#education-permissions). 

### <a name="app-permissions-to-enable-school-it-admins-to-consent"></a>Разрешения, которые должны предоставить приложению ИТ-администраторы учебного заведения 

Для развертывания приложений, интегрированных с API для образования в Microsoft Graph, ИТ-администраторы учебного заведения должны предоставить разрешения, запрашиваемые приложением. Повторный запрос появится, только если разрешения изменятся. Когда администратор предоставит разрешения, приложение будут подготовлено к работе для всех пользователей в клиенте.

Чтобы вызвать диалоговое окно для предоставления разрешений, используйте приведенный ниже вызов REST.

```
GET https://login.microsoftonline.com/{tenant}/adminconsent?
client_id={clientId}&state=12345&redirect_uri={redirectUrl}
```

|Параметр|Описание|
|:--------|:----------|
|Tenant|ИД клиента учебного заведения. Используйте полный идентификатор, например onmicrosoft.com.|
|clientId|Идентификатор клиента приложения.|
|redirectUrl|URL-адрес перенаправления приложения.|


## <a name="rostering"></a>Списки

API для работы со списком позволяют извлекать данные из клиента Office 365 учебного заведения, подготовленного с помощью [Microsoft School Data Sync](https://sds.microsoft.com/). Эти API предоставляют доступ к сведениям об учебных заведениях, секциях, преподавателях, учащихся и списках. Эти API поддерживают как сценарии только для приложений (синхронизацию), так и сценарии для приложений и пользователей (интерактивные). API, поддерживающие интерактивные сценарии, применяют политики RBAC на основе роли вызывающего API пользователя. Это обеспечивает согласованность API и минимальную область действия политики независимо от конфигурации администрирования в клиентах. Кроме того, API также предоставляют разрешения для образования, позволяющие настроить доступ к данным.

С помощью API для работы со списком можно предоставить пользователю приложения следующие сведения:

- его роль;
- предметы, которые он изучает или преподает;
- задания и сроки их выполнения.

API для работы со списком предоставляют следующие ключевые ресурсы:

- [educationSchool](educationschool.md) — учебное заведение;
- [educationClass](educationclass.md) — класс в учебном заведении;
- [educationTerm](educationterm.md) — определенная часть учебного года;
- [educationTeacher](educationteacher.md) — пользователи с основной ролью "Преподаватель";
- [educationStudent](educationstudent.md) — представляет пользователей с основной ролью "Учащийся".

API для работы со списком поддерживают следующие сценарии:

- [перечисление всех учебных заведений](../api/educationroot-list-schools.md); 
- [перечисление учебных заведений, в которых преподается определенный предмет](../api/educationclass-list-schools.md);
- [перечисление учебных заведений пользователя](../api/educationuser-list-schools.md);
- [получение всех классов](../api/educationroot_list_classes.md );
- [получение классов в учебном заведении](../api/educationschool-list-classes.md);
- [список классов пользователя](../api/educationuser-list-classes.md);
- [добавление классов в учебном заведении](../api/educationschool-post-classes.md);
- [получение учащихся и преподавателей класса](../api/educationclass-list-members.md);
- [добавление учащихся в класс](../api/educationclass-post-members.md); 
- [список преподавателей класса](../api/educationclass-list-teachers.md);
- [получение пользователей учебного заведения](../api/educationschool-list-users.md).

<!-- Should you list delete scenarios here as well? -->

## <a name="assignments"></a>Assignments 

Можно использовать education связанные назначения API-интерфейсы для интеграции с назначениями в группах Майкрософт. Группами Майкрософт в Office 365 для образовательных заведений на основании же образование интерфейсы API и обеспечивает пример использования что можно сделать с помощью интерфейсов API. Ваше приложение могут использовать эти API-интерфейсы для взаимодействия с назначениями на протяжении жизненного цикла назначения. 

Назначение API обеспечивают следующие основные ресурсы:

- [educationAssignment](educationassignment.md) - базовый объект назначения API. Представляет задачи или единицы трудозатрат, назначенных участником группы или учебы в классе как часть изучение.
- [educationSubmission](educationsubmission.md) - представляет ресурсы, отдельных пользователей (или групп) отправляет данные для назначения и связанные марки и свои отзывы и предложения для этого назначения.
- [educationResource](educationresource.md) - представляет, то есть объект обучающего присваивается или отправки. **EducationResource** связан с **educationAssignment** и/или **educationSubmission**.

Назначение интерфейсы API поддерживает следующие сценарии:

- [Создание назначения](../api/educationclass-post-assignments.md)
- [Опубликовать назначения](../api/educationassignment-publish.md)
- [Создание назначения ресурсов](../api/educationassignment-post-resources.md)
- [Создание ресурса отправки](../api/educationsubmission-post-resources.md)
- [Отправка назначения](../api/educationsubmission-submit.md) 
- [Unsubmit назначения](../api/educationsubmission-unsubmit.md)   
- [Вернуться к учебы оценки и обратная связь](../api/educationsubmission-return.md) 
- [Получите сведения о назначениях](../api/educationuser-list-assignments.md)

Ниже приведены некоторые наиболее распространенных случаев использования образования связанные назначения API-интерфейсы.

|Вариант использования|Описание|См. также|
|:-------|:----------|:-------|
|Создание назначения|Внешняя система позволяет создавать назначения для класса и ресурсы с подключением к назначению.|[Создание назначения](../api/educationassignment-post-resources.md)|
|Сведения о назначении чтения|Аналитика приложения можно получить сведения о назначениях и отправкой учебы, включая даты и оценки.|[Получение назначения](../api/educationassignment-get.md)|
|Отслеживание отправляемых учебы|Ваше приложение может предоставить учитель панели мониторинга, который показывает, сколько, отправляемых из студентов должны быть выражаемым числом.|[Отправка ресурсов](educationsubmission.md)|

## <a name="school-data-sync-management"></a>Управление синхронизацией данных School

[Синхронизация данных School](https://sds.microsoft.com/) помогает автоматизировать процесс импорта и синхронизации данных участников из учебы информационных систем с помощью Azure Active Directory (Azure AD) и Office 365. Интерфейсы управления синхронизации данных school в Microsoft Graph можно использовать для настройки синхронизации из CSV-файла или поддерживаемых SIS API соединителя.

Данные школа синхронизация поддержки API-интерфейсы управления следующие сценарии:

- [Список синхронизации профилей](../api/educationsynchronizationprofile-list.md)
- [Начало синхронизации профилей](../api/educationsynchronizationprofile-get.md)
- [Создание синхронизации профилей](../api/educationsynchronizationprofile-post.md)
- [Удаление синхронизации профилей](../api/educationsynchronizationprofile-delete.md)
- [Приостановка текущей синхронизации](../api/educationsynchronizationprofile-pause.md)
- [Возобновление приостановленной синхронизации](../api/educationsynchronizationprofile-resume.md)
- [Сброс синхронизации](../api/educationsynchronizationprofile-reset.md)
- [Запуск синхронизации переданных файлов](../api/educationsynchronizationprofile-start.md) 
- [Получение URL-адрес отправки](../api/educationsynchronizationprofile-uploadurl.md)
- [Получение состояния синхронизации](../api/educationsynchronizationprofilestatus-get.md)
- [Получение ошибки синхронизации](../api/educationsynchronizationerrors-get.md)


## <a name="next-steps"></a>Дальнейшие действия
Используйте education Microsoft Graph API-интерфейсы для создания решений образования, которые обращаются учащихся и списки school. Чтобы узнать больше:

- Изучите ресурсы и методы, наиболее полезные для вашего сценария.
- опробуйте API в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer).

<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/education-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
