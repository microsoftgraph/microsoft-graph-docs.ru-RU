---
title: Обновление teamsAppSettings
description: Обновление свойств объекта teamsAppSettings.
author: subray2014
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 5fdcc9fafe199e11881c59e65842c09d955eb74e
ms.sourcegitcommit: cf2b3c67cb9ce832944cfbac66171590bbbd83de
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/06/2022
ms.locfileid: "66645756"
---
# <a name="update-teamsappsettings"></a>Обновление teamsAppSettings
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств объекта [teamsAppSettings](../resources/teamsappsettings.md) .

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

>**Примечание:** Только глобальные администраторы и администраторы Teams могут вызывать этот API.

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|TeamworkAppSettings.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается|
|Приложение|Не поддерживается|

> [!NOTE]
> Разрешения TeamworkAppSettings.* могут не отображаться в портал Azure. Дополнительные сведения и способы их устранения см [. в статье об известных проблемах](/graph/known-issues#teamworkappsettings-permissions-are-not-visible-in-the-azure-portal).

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /teamwork/teamsAppSettings
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]


|Свойство|Тип|Описание|
|:---|:---|:---|
|isChatResourceSpecificConsentEnabled|Логическое|Указывает, включено ли для клиента согласие на чаты и собрания для конкретного ресурса. Если значение равно true, приложения Teams, которые разрешены в клиенте и требуют разрешений для конкретных ресурсов, можно устанавливать в чатах и собраниях. Если задано значение false, установка любого приложения Teams, для которого требуются разрешения конкретного ресурса в чате или на собрании, будет заблокирована.|



## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.

## <a name="examples"></a>Примеры

### <a name="example-1-enable-installation-of-apps-that-require-resource-specific-consent-in-chatsmeetings"></a>Пример 1. Включение установки приложений, для которых требуется согласие конкретного ресурса, в чатах или собраниях.

#### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "update_teamsappsettings"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/teamwork/teamsAppSettings
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.teamsAppSettings",
  "isChatResourceSpecificConsentEnabled": "true"
}
```

#### <a name="response"></a>Отклик

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a>См. также

- [Согласие для определенных ресурсов](/microsoftteams/platform/graph-api/rsc/resource-specific-consent)