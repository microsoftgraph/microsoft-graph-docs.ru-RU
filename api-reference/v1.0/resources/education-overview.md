---
title: Работа с интерфейсами API для образования в Microsoft Graph
description: API для образования в Microsoft Graph дополняют ресурсы и данные Microsoft 365 сведениями, актуальными для учебных заведений, учащихся, преподавателей, классов и списков. Это упрощает создание решений, интегрируемых с образовательными ресурсами.
ms.localizationpriority: high
author: mmast-msft
ms.prod: education
doc_type: conceptualPageType
ms.openlocfilehash: d7d4fe8b5040221cc7d54569af1cfc87429ef852
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60688971"
---
# <a name="working-with-education-apis-in-microsoft-graph"></a>Работа с интерфейсами API для образования в Microsoft Graph

API для образования в Microsoft Graph дополняют ресурсы и данные Microsoft 365 сведениями, актуальными для учебных заведений, учащихся, преподавателей, классов и списков. Это упрощает создание решений, интегрируемых с образовательными ресурсами.

API для образования включают ресурсы для управления списком и ресурсы заданий, которые можно использовать для взаимодействия с соответствующими службами в Microsoft Teams. С помощью этих ресурсов можно управлять списком пользователей учебного учреждения.

## <a name="authorization"></a>Авторизация

Чтобы вызывать API для образования в Microsoft Graph, приложению необходимо получить маркер доступа. Подробные сведения о маркерах доступа см. в статье [Получение маркеров доступа для вызова Microsoft Graph](/graph/auth/). Приложению также потребуются соответствующие разрешения. Дополнительные сведения см. в разделе [Разрешения для образования](/graph/permissions-reference#education-permissions).

### <a name="app-permissions-to-enable-school-it-admins-to-consent"></a>Разрешения, которые должны предоставить приложению ИТ-администраторы учебного заведения

Для развертывания приложений, интегрированных с API для образования в Microsoft Graph, ИТ-администраторы учебного заведения должны предоставить разрешения, запрашиваемые приложением. Повторный запрос появится, только если разрешения изменятся. Когда администратор предоставит разрешения, приложение будет подготовлено к работе для всех пользователей в клиенте.

Чтобы отобразить диалоговое окно для предоставления разрешений, используйте приведенный ниже вызов REST.

```http
GET https://login.microsoftonline.com/{tenant}/adminconsent?
client_id={clientId}&state=12345&redirect_uri={redirectUrl}
```

| Параметр   | Описание                                                               |
| :---------- | :------------------------------------------------------------------------ |
| Tenant      | ИД клиента учебного заведения. Используйте полный идентификатор, например onmicrosoft.com. |
| clientId    | Идентификатор клиента приложения.                                                     |
| redirectUrl | URL-адрес перенаправления приложения.                                                         |

## <a name="rostering"></a>Списки

API для работы со списком позволяют извлекать данные из клиента Microsoft 365 учебного заведения, подготовленного с помощью [Microsoft School Data Sync](https://sds.microsoft.com/). Эти API предоставляют доступ к сведениям об учебных заведениях, секциях, преподавателях, учащихся и списках. Эти API поддерживают как сценарии только для приложений (синхронизацию), так и сценарии для приложений и пользователей (интерактивные). API, поддерживающие интерактивные сценарии, применяют политики RBAC на основе роли вызывающего API пользователя. Это обеспечивает согласованность API и минимальную область действия политики независимо от конфигурации администрирования в клиентах. Кроме того, API также предоставляют разрешения для образования, позволяющие настроить доступ к данным.

С помощью API для работы со списком можно предоставить пользователю приложения следующие сведения:

- его роль;
- предметы, которые он изучает или преподает;
- задания и сроки их выполнения.

API для работы со списком предоставляют следующие ключевые ресурсы:

- [educationSchool](educationschool.md) — учебное заведение;
- [educationClass](educationclass.md) — класс в учебном заведении;
- [educationTerm](educationterm.md) — определенная часть учебного года;
- [educationTeacher](educationteacher.md) — пользователь с основной ролью "Преподаватель";
- [educationStudent](educationstudent.md) — пользователь с основной ролью "Учащийся".

API для работы со списком поддерживают следующие сценарии:

- [перечисление всех учебных заведений](../api/educationschool-list.md);
- [перечисление учебных заведений, в которых преподается определенный предмет](../api/educationclass-list-schools.md);
- [перечисление учебных заведений пользователя](../api/educationuser-list-schools.md);
- [получение всех классов](../api/educationclass-list.md);
- [получение классов в учебном заведении](../api/educationschool-list-classes.md);
- [список классов пользователя](../api/educationuser-list-classes.md);
- [добавление классов в учебном заведении](../api/educationschool-post-classes.md);
- [получение учащихся и преподавателей класса](../api/educationclass-list-members.md);
- [добавление учащихся в класс](../api/educationclass-post-members.md);
- [список преподавателей класса](../api/educationclass-list-teachers.md);
- [получение пользователей учебного заведения](../api/educationschool-list-users.md).

<!-- Should you list delete scenarios here as well? -->

## <a name="assignments"></a>Задания

Вы можете использовать API для образования, связанные с заданиями, чтобы выполнять интеграцию с заданиями в Microsoft Teams. Microsoft Teams в Microsoft 365 для образования основан на тех же API для образования и предоставляет вариант использования API. Ваше приложение может использовать эти API для взаимодействия с заданиями в течение всего жизненного цикла задания. 

API заданий предоставляют следующие ключевые ресурсы.

- [educationAssignment](educationassignment.md) — основной объект API заданий. Представляет задачу или единицу работы, назначенную учащемуся или участнику команды в классе в рамках его исследования.
- [educationSubmission](educationsubmission.md) — представляет ресурсы, отправляемые человеком (или группой) в рамках задания, а также связанные оценки и отзывы по этому заданию.
- [educationResource](educationresource.md) — представляет объект обучения, который назначается или отправляется. Объект **educationResource** связан с **educationAssignment** и/или **educationSubmission**.

API заданий поддерживают следующие сценарии.

- [Создание задания](../api/educationclass-post-assignment.md)
- [Публикация задания](../api/educationassignment-publish.md)
- [Создание ресурса задания](../api/educationassignment-post-resource.md)
- [Создание ресурса сданной работы](../api/educationsubmission-post-resources.md)
- [Отправка задания](../api/educationsubmission-submit.md)
- [Отмена отправки задания](../api/educationsubmission-unsubmit.md)
- [Возвращение оценок и отзывов учащемуся](../api/educationsubmission-return.md)

Ниже приводится несколько распространенных вариантов использования API для образования, связанных с заданиями.

| Вариант использования                    | Описание                                                                                                         | См. также                                                          |
| :-------------------------- | :------------------------------------------------------------------------------------------------------------------ | :---------------------------------------------------------------- |
| Создание заданий          | Внешняя система может создать задание для класса и вложить ресурсы для задания.                   | [Создание задания](../api/educationassignment-post-resource.md) |
| Чтение сведений о задании | Приложение аналитики может получать сведения о заданиях и сданных работах учащихся, включая даты и оценки. | [Получение задания](../api/educationassignment-get.md)               |
| Отслеживание сданных работ учащихся   | Ваше приложение может предоставлять информационную панель для преподавателей, указывающую количество сданных работ учащихся, которые нужно оценить.           | [Ресурс сданной работы](educationsubmission.md)                     |

## <a name="whats-new"></a>Новые возможности

Узнайте о [новых функциях и обновлениях](/graph/whats-new-overview) для этого набора API.

## <a name="next-steps"></a>Дальнейшие действия

С помощью API для образования в Microsoft Graph вы можете создавать решения с доступом к спискам пользователей учебного заведения. Дополнительные сведения:

- Изучите ресурсы и методы, наиболее полезные для вашего сценария.
- опробуйте API в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer).
