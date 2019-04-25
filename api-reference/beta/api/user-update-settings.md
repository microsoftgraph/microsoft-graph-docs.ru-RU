---
title: Обновление параметров
description: 'Обновление свойств объекта Settings. '
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5536eb096ae963990e4a06f6fc95e273fd4d1557
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32547629"
---
# <a name="update-settings"></a>Обновление параметров

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств объекта [Settings](../resources/user-settings.md) . Пользователи в одной организации могут иметь различные параметры в зависимости от их предпочтения или политики Организации. Чтобы получить текущие параметры пользователя, просмотрите [параметры текущей учетной записи пользователя](user-get-settings.md). 

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | User. ReadWrite, User. ReadWrite. ALL   |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | User.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

```http
PATCH /me/settings
```

Запрос с идентификатором пользователя или userPrincipalName доступен только пользователю или пользователем с разрешениями User. ReadWrite. ALL. Чтобы узнать больше, ознакомьтесь [](/graph/permissions-reference)с разрешениями. 

```http
PATCH /users/{id | userPrincipalName}/settings/
```

## <a name="request-headers"></a>Заголовки запросов

| Заголовок       | Значение|
|:-----------|:------|
| Авторизация  | Bearer {токен}. Обязательный.  |
| Content-Type  | application/json  |

## <a name="request-body"></a>Текст запроса

В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|Контрибутионтоконтентдисковеридисаблед|Логический|Установите значение true, чтобы запретить представителю доступ [](../resources/insights-trending.md) к API тенденций и отключить доступ к документам в Office delve для пользователя. Значение true также влияет на релевантность контента, отображаемого в Office 365, например, Рекомендуемые сайты в SharePoint Home и представление обнаружение в OneDrive для бизнеса содержат менее релевантные результаты. Этот параметр отражает состояние элемента управления в [Office delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).|

## <a name="example"></a>Пример 

##### <a name="request"></a>Запрос

Ниже приведен пример запроса на отказаться от участия пользователя в delve и отказаться от его участия в релевантности контента для всей Организации.

```http
PATCH https://graph.microsoft.com/beta/me/settings
Content-type: application/json
Content-length: 37

{
  "contributionToContentDiscoveryDisabled": true
}
```

##### <a name="response"></a>Отклик

Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "contributionToContentDiscoveryAsOrganizationDisabled": false,
  "contributionToContentDiscoveryDisabled": true
}
```

#### <a name="batch-request"></a>Пакетный запрос

Кроме того, можно отказаться от использования нескольких пользователей из delve и отказаться от их вклада в релевантность содержимого для всей Организации с помощью пакетного запроса.
Для получения дополнительных сведений см [Пакетная обработка JSON](/graph/json-batching).

**Важно!** только члены группы ролей " [Управление организацией](https://support.office.com/article/permissions-in-the-office-365-security-compliance-center-d10608af-7934-490a-818e-e68f17d0e9c1?ui=en-US&rs=en-US&ad=US) " могут обновлять нескольких пользователей. 


<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/user-update-settings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
