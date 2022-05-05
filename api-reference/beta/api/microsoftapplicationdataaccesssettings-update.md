---
title: Обновление microsoftApplicationDataAccessSettings
description: Обновление свойств объекта microsoftApplicationDataAccessSettings.
author: ttomi
ms.localizationpriority: medium
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 411a1b8cad849979cb3c0d49500c45d1e452037e
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65212406"
---
# <a name="update-microsoftapplicationdataaccesssettings"></a>Обновление microsoftApplicationDataAccessSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновите параметры в объекте [microsoftApplicationDataAccessSettings](../resources/microsoftapplicationdataaccesssettings.md), которые задают доступ из приложений Майкрософт к Microsoft 365 данных пользователей в организации.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|Organization.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /organization/{organizationId}/settings/microsoftApplicationDataAccess
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
|isEnabledForAllMicrosoftApplications|Логический|Если задано значение ,`true`все пользователи в организации могут получить доступ к приложению Майкрософт Microsoft 365 данных, к которым пользователь был авторизован. Приложение Майкрософт может быть приложением Microsoft 365 (например, Excel, Outlook) или не Microsoft 365 приложением (например, Edge). Значение по умолчанию: `true`. <br> Этот доступ можно отключить для подмножества пользователей в группе безопасности Azure Active Directory (Azure AD), указав группу в свойстве **disabledForGroup**. <br> Если задано значение `false`,пользователи могут получить доступ к Microsoft 365 только в Microsoft 365 приложении.|
|disabledForGroup|Строка|Идентификатор группы безопасности Azure AD, члены которой могут получать доступ к Microsoft 365 с помощью только Microsoft 365 приложений, но не других приложений Майкрософт, таких как Edge. <br> Это применимо только в том случае, если **для isEnabledForAllMicrosoftApplications** задано значение `true`.|

## <a name="response"></a>Ответ

В случае успешного выполнения `200 OK` этот метод возвращает код отклика и обновленный объект [microsoftApplicationDataAccessSettings](../resources/microsoftapplicationdataaccesssettings.md) в теле отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

В следующем примере запроса показано, как администратор обновляет параметр конфиденциальности **disabledForGroup**, чтобы запретить пользователям в определенной группе Azure AD доступ к данным Microsoft 365 с помощью приложений Майкрософт, которые не являются частью Microsoft 365.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_microsoftapplicationdataaccesssettings"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/organization/{organizationId}/settings/microsoftApplicationDataAccess
Content-Type: application/json

{
  "disabledForGroup": "edbfe4fb-ec70-4300-928f-dbb2ae86c981"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-microsoftapplicationdataaccesssettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-microsoftapplicationdataaccesssettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-microsoftapplicationdataaccesssettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-microsoftapplicationdataaccesssettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-microsoftapplicationdataaccesssettings-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-microsoftapplicationdataaccesssettings-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.microsoftApplicationDataAccessSettings",
  "name": "update_microsoftapplicationdataaccesssettings"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.microsoftApplicationDataAccessSettings",
  "isEnabledForAllMicrosoftApplications": true,
  "disabledForGroup": "edbfe4fb-ec70-4300-928f-dbb2ae86c981"
}
```
