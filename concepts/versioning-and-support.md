---
title: 'Политики поддержки и внесения критических изменений в Microsoft Graph, а также доступные версии '
description: В этой статье описаны политики поддержки и внесения критических изменений в Microsoft Graph, а также доступные версии API Microsoft Graph.
localization_priority: Priority
ms.openlocfilehash: 47d0ec66fc335a50826d94511c8f9e6551c927a6
ms.sourcegitcommit: 3c8a92d89ac60a48cb63449976b1c3c2c6302281
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/16/2020
ms.locfileid: "44744006"
---
# <a name="versioning-support-and-breaking-change-policies-for-microsoft-graph"></a>Политики поддержки и внесения критических изменений в Microsoft Graph, а также доступные версии

В этой статье описаны политики поддержки и внесения критических изменений в Microsoft Graph, а также доступные версии API Microsoft Graph.

## <a name="support-policy-and-deprecation-information"></a>Политика поддержки и объявление о прекращении поддержки

Microsoft Graph придерживается политики [Microsoft Lifecycle](https://support.microsoft.com/lifecycle).

As new versions of the Microsoft Graph REST APIs and Microsoft Graph SDKs are released, earlier versions will be retired. Microsoft will declare a version as deprecated at least 24 months in advance of retiring an API or an SDK.

После увеличения основного номера версии API (например, с 1.0 до 2.0) текущая версия (в этом примере — 1.0) будет объявлена устаревшей, и ее поддержка будет прекращена через 24 месяца после объявления. В политику могут быть внесены исключения, если возникнут проблемы с безопасностью или работоспособностью службы.

Когда API помечен как недопустимый, настоятельно рекомендуем как можно быстрее переходить на последнюю версию. В некоторых случаях мы будем объявлять, что новые приложения должны быть запущены с использованием новых API некоторое время спустя после того как исходные API становятся недопустимыми. В таких случаях только активные приложения, которые в настоящее время используют недопустимые API-интерфейсы могут продолжать их использование.

### <a name="api-contract-and-non-backward-compatible-changes"></a>Изменения в контракте API и изменения, не совместимые с прежними версиями

Microsoft Graph has a log of changes across versions. These changes are listed in the [Microsoft Graph Changelog](changelog.md). As new functionality and data is added to Microsoft Graph, we will increment the API version number for any non-backward compatible changes to the API.

Примеры изменений, не совместимых с прежними версиями:

- изменения URL-адреса или основного запроса/ответа, связанного с ресурсом;
- удаление, переименование или изменение типа объявленного свойства;
- удаление или переименование API или их параметров;
- добавление обязательного заголовка запроса.

Примеры обратно совместимых изменений:

- добавление свойств, которые допускают значение null или имеют значение по умолчанию;
- добавление элемента в перечисление;
- удаление, переименование или изменение типа открытого расширения;
- удаление, переименование или изменение типа заметки;
- разбиение существующих коллекций на страницы;
- изменения кодов ошибок;
- изменения порядка свойств;
- изменения длины или формата непрозрачных строк, таких как идентификаторы ресурсов.

>**Note:** Over time, we will update the list of backward compatible changes. If you generate your own client proxies (like WCF clients), our guidance is that your client applications should be prepared to receive properties and derived types not previously defined by the Microsoft Graph API service. Microsoft Graph API follows the guidance described in the [Model Versioning](https://github.com/Microsoft/api-guidelines/blob/master/Guidelines.md#12-versioning) section in the [Microsoft REST API guidelines](https://github.com/microsoft/api-guidelines/).

## <a name="versions"></a>Версии

В настоящее время доступны указанные ниже версии API Microsoft Graph.

### <a name="beta-version"></a>Бета-версия
Бета-версия API Microsoft Graph, доступная в разделе ниже, `https://graph.microsoft.com/beta` содержит функции, находящиеся _** на стадии тестирования **_. Документацию по API бета-версии см. в [справочнике по конечной точке бета-версии Microsoft Graph](/graph/api/overview?view=graph-rest-beta). Время от времени в бета-версию могут вноситься критические изменения. Не используйте API /beta в рабочих приложениях.

We make no guarantees that a beta feature will be promoted to the current version. When the Microsoft Graph API team believes that a beta feature is ready for general availability (GA), we will add that feature to the latest current version. If the promotion of the feature would result in a breaking change to the current version, the version number will be incremented, with the new version becoming the current version.
Our developer community can post feature request on [UserVoice](https://officespdev.uservoice.com/), including requests for new features as well as requests to promote existing beta APIs to the current version.

### <a name="current-version"></a>Текущая версия

The current version of Microsoft Graph is v1.0. Exposed under `https://graph.microsoft.com/v1.0`, the Microsoft Graph API /v1.0 version contains features that are generally available and ready for production use. You can browse the documentation for the v1.0 APIs in the table of contents.

### <a name="deprecated-and-unsupported-versions"></a>Устаревшие и неподдерживаемые версии

В настоящий момент нет устаревших версий Microsoft Graph.

## <a name="terms-of-use"></a>Условия использования

Используя API Microsoft Graph, вы принимаете [Условия использования API Microsoft](/legal/microsoft-apis/terms-of-use?context=/graph/context).

Your feedback is important to us. Connect with us on [StackOverflow](https://stackoverflow.com/questions/tagged/microsoftgraph?sort=newest). Tag your questions with [microsoft-graph].
