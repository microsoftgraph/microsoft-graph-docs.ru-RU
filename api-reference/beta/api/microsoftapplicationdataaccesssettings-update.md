---
title: Обновление microsoftApplicationDataAccessSettings
description: Обновление свойств объекта MicrosoftApplicationDataAccessSettings.
author: ttomi
ms.localizationpriority: medium
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: d7031fefb9f90718dc0e0fb66714cb933fa9dfe9
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589824"
---
# <a name="update-microsoftapplicationdataaccesssettings"></a>Обновление microsoftApplicationDataAccessSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление параметров объекта [MicrosoftApplicationDataAccessSettings](../resources/microsoftapplicationdataaccesssettings.md), который указывает доступ из приложений Майкрософт к Microsoft 365 пользовательских данных в организации.

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
|isEnabledForAllMicrosoftApplications|Логическое|Если установлено`true`, все пользователи в организации могут получить доступ в приложении Майкрософт к любым Microsoft 365 данным, к данным, к которые пользователь получил разрешение на доступ. Приложение Microsoft может быть приложением Microsoft 365 (например, Excel, Outlook) или не Microsoft 365 приложением (например, Edge). Значение по умолчанию: `true`. <br> Этот доступ можно отключить для подмножество пользователей в группе безопасности Azure Active Directory Azure AD, указав группу в свойстве **disabledForGroup**. <br> Если установлено`false`, пользователи могут получать доступ к Microsoft 365 данным только в Microsoft 365 приложении.|
|disabledForGroup|Строка|ID группы безопасности Azure AD, члены которой могут получать доступ к Microsoft 365 с помощью только Microsoft 365 приложений, но не других приложений Майкрософт, таких как Edge. <br> Это применимо только в том случае, если **установлено для isEnabledForAllMicrosoftApplications** `true`.|

## <a name="response"></a>Отклик

В случае успеха `200 OK` этот метод возвращает код ответа и обновленный [объект MicrosoftApplicationDataAccessSettings](../resources/microsoftapplicationdataaccesssettings.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

В следующем примере показано, как администратор обновляет параметр конфиденциальности **disabledForGroup**, чтобы запретить пользователям определенной группы Azure AD получать доступ к Microsoft 365 с помощью приложений Майкрософт, не включающих Microsoft 365.

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
