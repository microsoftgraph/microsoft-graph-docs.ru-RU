---
title: Обновление mobileAppManagementPolicy
description: Обновление свойств объекта политики управления мобильными приложениями.
author: ravennMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: b553a291ce986a3084403c55f3c991fb260c4828
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401647"
---
# <a name="update-mobileappmanagementpolicy"></a>Обновление mobileAppManagementPolicy

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств объекта [mobilityManagementPolicy.](../resources/mobilitymanagementpolicy.md)

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|Policy.Read.All, Policy.ReadWrite.MobilityManagement|
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.|
|Для приложений | Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /policies/mobileAppManagementPolicies/{id}
```

## <a name="request-headers"></a>Заголовки запросов

|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса

В теле запроса поставляем JSON-представление объекта [mobilityManagementPolicy.](../resources/mobilitymanagementpolicy.md)

В теле запроса укажи значения для перечисленных ниже полей, которые должны быть обновлены. **Примечание:** С другими свойствами нельзя использовать `PATCH` `appliesTo` операцию.

|Свойство|Тип|Описание|
|:---|:---|:---|
|appliesTo|policyScope|Определяет группы, к которые применяется этот параметр политики. Возможные значения: `none` , `all` , `selected` **Важно: не** может использоваться при `selected` указании этого свойства. Используйте [includedGroups для](../api/mobileappmanagementpolicies-post-includedgroups.md) добавления определенных групп.|
|complianceUrl|String|URL-адрес соответствия приложению управления мобильностью|
|discoveryUrl|String|Обнаружение URL-адреса приложения для управления мобильностью|
|termsOfUseUrl|String|Условия использования URL-адреса приложения для управления мобильностью|

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика и обновленный объект `200 OK` [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "update_mobilitymanagementpolicy"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/policies/mobileAppManagementPolicies/ab90bacf-55a3-4a3e-839a-aa4b74e4f020
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.mobilityManagementPolicy",
  "complianceUrl": "https://portal.mg.contoso.com/?portalAction=Compliance",
  "discoveryUrl": "https://enrollment.mg.contoso.com/enrollmentserver/discovery.svc",
  "termsOfUseUrl": "https://portal.mg.contoso.com/TermsofUse.aspx"
}
```

### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
