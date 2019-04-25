---
title: Работа с интерфейсами API для образования в Microsoft Graph
description: API для образования в Microsoft Graph улучшают ресурсы и данные Office 365 с помощью информации, которая относится к обучающим, учащимся, преподавателям, классам, заявкам и назначениям. Это упрощает создание решений, интегрируемых с образовательными ресурсами.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 9e106da7eb717a091941e16f4a70af8a012802f3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534873"
---
# <a name="working-with-education-apis-in-microsoft-graph"></a>Работа с интерфейсами API для образования в Microsoft Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

API для образования в Microsoft Graph улучшают ресурсы и данные Office 365 с помощью информации, которая относится к обучающим, учащимся, преподавателям, классам, заявкам и назначениям. Это упрощает создание решений, интегрируемых с образовательными ресурсами.

API для образования включают в себя список ресурсов и ресурсов назначений, которые можно использовать для взаимодействия со службами подбора и назначения в Microsoft Teams. Эти ресурсы можно использовать для управления списком учебного заведения и автоматизации назначений учащихся.

## <a name="authorization"></a>Авторизация

Чтобы вызывать API для образования в Microsoft Graph, приложению необходимо получить маркер доступа. Подробные сведения о маркерах доступа см. в статье [Получение маркеров доступа для вызова Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview). Приложению также потребуются соответствующие разрешения. Дополнительные сведения см. в разделе [Разрешения для образования](/graph/permissions-reference#education-permissions). 

### <a name="app-permissions-to-enable-school-it-admins-to-consent"></a>Разрешения, которые должны предоставить приложению ИТ-администраторы учебного заведения 

Для развертывания приложений, интегрированных с API для образования в Microsoft Graph, ИТ-администраторы учебного заведения должны предоставить разрешения, запрашиваемые приложением. Повторный запрос появится, только если разрешения изменятся. Когда администратор предоставит разрешения, приложение будет подготовлено к работе для всех пользователей в клиенте.

Чтобы запустить диалоговое окно согласия, используйте следующий вызов REST.

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

## <a name="assignments"></a>Задания 

Для интеграции с назначениями в Microsoft Teams можно использовать API для образования, связанный с назначениями. Microsoft Teams в Office 365 для образовательных учреждений базируется на тех же интерфейсах API для образования, а также предоставляет вариант использования API. Приложение может использовать эти API для взаимодействия с назначениями во время жизненного цикла назначения. 

API назначения предоставляют следующие ключевые ресурсы:

- [educationAssignment](educationassignment.md) — основной объект API назначений. Представляет задачу или единицу работы, назначенную студенту или участнику команды в классе в ходе их изучения.
- [educationSubmission](educationsubmission.md) — представляет ресурсы, которые индивидуальные (или групповые) отправляют для назначения, а также связанные с ними оценки и отзывы для этого назначения.
- [едукатионресаурце](educationresource.md) — представляет объект Learning, который назначается или отправляется. Объект **едукатионресаурце** связан с **educationAssignment** и/или **educationSubmission**.

API назначения поддерживают следующие сценарии:

- [Создание задания](../api/educationclass-post-assignments.md)
- [Публикация задания](../api/educationassignment-publish.md)
- [Создание ресурса задания](../api/educationassignment-post-resources.md)
- [Создание ресурса отправки](../api/educationsubmission-post-resources.md)
- [Назначение для отПравки](../api/educationsubmission-submit.md) 
- [Отправку назначения](../api/educationsubmission-unsubmit.md)   
- [Возврат оценок и обратная связь для учащихся](../api/educationsubmission-return.md) 
- [Получение сведений о назначении](../api/educationuser-list-assignments.md)

Ниже приведены некоторые распространенные варианты использования API образования, связанного с назначениями.

|Вариант использования|Описание|См. также|
|:-------|:----------|:-------|
|Создание назначений|Внешняя система может создать назначение для класса и присоединить ресурсы к назначению.|[Создание задания](../api/educationassignment-post-resources.md)|
|Чтение сведений о назначениях|Приложение аналитики может получать сведения о назначениях и отправок учащихся, в том числе даты и оценки.|[Получение задания](../api/educationassignment-get.md)|
|Отслеживание отправок учащихся|Ваше приложение может предоставить панель мониторинга преподавателя, в которой показано, сколько отправок от учащихся должно быть продолжено.|[Ресурс отправки](educationsubmission.md)|

## <a name="school-data-sync-management"></a>Управление синхронизацией данных School

[School Data Sync](https://sds.microsoft.com/) помогает автоматизировать процесс импорта и синхронизации данных списков из информационных систем учащихся с Azure Active Directory (Azure AD) и Office 365. С помощью API School Data Sync Managements в Microsoft Graph можно настроить синхронизацию с помощью CSV-файла или поддерживаемого соединителя API SIS.

API управления для School Data Sync поддерживают следующие сценарии:

- [Профили синхронизации списка](../api/educationsynchronizationprofile-list.md)
- [Получение профиля синхронизации](../api/educationsynchronizationprofile-get.md)
- [Создание профиля синхронизации](../api/educationsynchronizationprofile-post.md)
- [Удаление профиля синхронизации](../api/educationsynchronizationprofile-delete.md)
- [ПриОстановка текущей синхронизации](../api/educationsynchronizationprofile-pause.md)
- [ВозОбновление приостановленной синхронизации](../api/educationsynchronizationprofile-resume.md)
- [Сброс синхронизации](../api/educationsynchronizationprofile-reset.md)
- [Запуск синхронизации для отправленных файлов](../api/educationsynchronizationprofile-start.md) 
- [Получение URL-адреса отправки](../api/educationsynchronizationprofile-uploadurl.md)
- [Получение состояния синхронизации](../api/educationsynchronizationprofilestatus-get.md)
- [Получение ошибок синхронизации](../api/educationsynchronizationerrors-get.md)


## <a name="next-steps"></a>Дальнейшие действия
Используйте API Microsoft Graph для образования, чтобы создавать решения для образования, которые получают доступ к назначениям учащихся и их спискам учебного заведения. Чтобы узнать больше:

- Изучите ресурсы и методы, наиболее полезные для вашего сценария.
- Опробуйте API в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer).

<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/education-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
