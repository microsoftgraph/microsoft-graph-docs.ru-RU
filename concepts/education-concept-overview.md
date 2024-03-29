---
title: Обзор API для образования
description: Используйте образовательный API в Microsoft Graph для создания решений, которые интегрируются с образовательными ресурсами для сценариев в классе, таких как списки и задания.
author: mmast-msft
ms.localizationpriority: high
ms.prod: education
ms.custom: scenarios:getting-started
ms.openlocfilehash: cddc7efd0d5242f68224c3909d0d93e2b55616d2
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66440896"
---
# <a name="education-api-overview"></a>Обзор API для образования

API в Microsoft Graph дополняет ресурсы Microsoft 365 сведениями, актуальными для учебных заведений, включая данные об учреждениях, классах, пользователях (учащихся и преподавателях), заданиях и сданных работах. Это упрощает создание решений, интегрируемых с образовательными ресурсами, для различных сценариев в учебных заведениях и аудиториях.

> [!VIDEO https://www.youtube-nocookie.com/embed/EnDM7KMTEqQ]

## <a name="why-integrate-with-education-scenarios"></a>Зачем нужна интеграция со сценариями образования?

### <a name="build-applications-that-are-aware-of-class-roster"></a>Создавайте приложений, работающие со списком курса

Большинство разработчиков программного обеспечения быстро понимают, что список курса — один из важнейших ресурсов для работы приложения. Как правило, он скрыт в информационной системе для учащихся (SIS). Каждый раз, когда преподаватели приносят в класс новое приложение, им приходится вручную импортировать в него данные о составе. Многие независимые поставщики программного обеспечения решают эту проблему, подключаясь к SIS для импорта данных о составе. Учитывая, что на рынке доступны сотни информационных систем для учащихся, где используются собственные форматы, это может оказаться непростой задачей.

[Microsoft School Data Sync](https://sds.microsoft.com/) в сочетании с API для списков курсов помогает разработчикам приложений и учебным заведениям решить эту проблему. Вот некоторые сценарии, которые поддерживают API для списков курсов:

- [получение всех классов в учебном заведении](/graph/api/educationschool-list-classes);
- [получение всех пользователей в классе](/graph/api/educationclass-list-members);
- [получение всех классов, в которых я преподаю](/graph/api/educationuser-list-classes).


### <a name="use-microsoft-teams-to-create-class-assignments-in-an-assignments-tab"></a>Используйте Microsoft Teams для создания заданий для классов на соответствующей вкладке

Вы можете использовать API для образования, связанные с заданиями, чтобы выполнять интеграцию с заданиями в Microsoft Teams. Microsoft Teams в Microsoft 365 для образования основан на тех же API для образования и предоставляет вариант использования API. Ваше приложение может использовать эти API для взаимодействия с заданиями в течение всего жизненного цикла задания.

API заданий предоставляют следующие ключевые ресурсы.

- [educationAssignment](/graph/api/resources/educationassignment): основной объект API заданий. Представляет задачу или единицу работы, назначенную учащемуся или участнику команды в классе в рамках его исследования.
- [educationSubmission](/graph/api/resources/educationsubmission): представляет ресурсы, отправляемые человеком (или группой) в рамках задания, а также связанные оценки и отзывы по этому заданию.
- [educationResource](/graph/api/resources/educationresource): представляет объект обучения, который назначается или отправляется. Объект **educationResource** связан с **educationAssignment** и/или **educationSubmission**.

При помощи API заданий приложение может взаимодействовать со службой заданий вне Microsoft Teams. Microsoft Teams займется распространением, датами выполнения и оценками, а ваша система обеспечит для учащихся удобные условия обучения.

Ниже приведены примеры сценариев, работу которых обеспечивает API заданий:

- [добавление задания, связанного с вашим приложением](/graph/api/educationclass-post-assignments); 
- [назначение отдельным учащимся результатов, например, оценок, за задания, связанные с вашим приложением;](/graph/api/educationoutcome-update)
- [создание информационной панели с датами выполнения заданий](/graph/api/educationclass-list-assignments).

### <a name="enable-school-admins-to-manage-identity-and-roster-sync-using-school-data-sync-management-preview"></a>Предоставьте администраторам учебного заведения возможность управлять синхронизацией удостоверений и списков при помощи School Data Sync Management (ознакомительная версия)

[Синхронизация сведений о школе](https://sds.microsoft.com/) помогает автоматизировать процесс импорта и синхронизации данных об удостоверениях и списках учащихся из информационных систем для учащихся с Azure Active Directory (Azure AD) и Microsoft 365. При синхронизации этих сведений вы можете использовать API для импорта информации о списке класса в приложения. 

Если вы настраиваете интеграцию информационной системы для учащихся со School Data Sync, можете воспользоваться [API для управления SDS](/graph/api/resources/educationsynchronizationprofile) в Microsoft Graph, чтобы настроить синхронизацию из CSV-файла или поддерживаемого соединителя API для SIS.

API управления School Data Sync поддерживают полноценные сценарии управления синхронизацией, например:

- [Создание профиля, автоматически запускающего синхронизацию](/graph/api/educationsynchronizationprofile-post).
- управление жизненным циклом синхронизации при помощи операций [pause](/graph/api/educationsynchronizationprofile-pause), [resume](/graph/api/educationsynchronizationprofile-resume) и [reset](/graph/api/educationsynchronizationprofile-reset).

## <a name="api-reference"></a>Справочные материалы по API

Ищете справочные материалы по API для этой службы?

- [API для образования в Microsoft Graph 1.0](/graph/api/resources/education-overview?view=graph-rest-1.0&preserve-view=true)
- [API для образования в бета-версии Microsoft Graph](/graph/api/resources/education-overview?view=graph-rest-beta&preserve-view=true)

## <a name="next-steps"></a>Дальнейшие действия

Прежде чем приступить к использованию API для образования, ознакомьтесь со следующими статьями:
- [Использование API для списков курсов](/graph/api/resources/education-overview)
- [Использование API заданий](/graph/api/resources/educationassignment)
- [Использование API управления SDS](/graph/api/resources/educationsynchronizationprofile)

Опробуйте API для образования в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer).

Ознакомьтесь со следующими примерами, связанными с образованием:
- [Пример единого входа и составления списков на .NET](https://github.com/OfficeDev/O365-EDU-AspNetMVC-Samples)
- [Пример использования API для управления профилями](https://github.com/OfficeDev/O365-EDU-SDS-AspNetMVC-Samples)