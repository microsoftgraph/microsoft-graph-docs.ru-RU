---
title: Перечисление emailThreatSubmissionPolicies
description: Получение списка объектов emailThreatSubmissionPolicy и их свойств.
author: caigen
ms.localizationpriority: medium
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 445660425e0c71fc0217006ab8d81e1f25cc9c34
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856723"
---
# <a name="list-emailthreatsubmissionpolicies"></a>Перечисление emailThreatSubmissionPolicies
Пространство имен: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение списка объектов [emailThreatSubmissionPolicy](../resources/security-emailthreatsubmissionpolicy.md) и их свойств.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|ThreatSubmission.Read, ThreatSubmission.ReadWrite, ThreatSubmission.Read.All, ThreatSubmission.ReadWrite.All, ThreatSubmissionPolicies.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается|
|Приложение|ThreatSubmission.Read.All, ThreatSubmission.ReadWrite.All, ThreatSubmissionPolicy.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET security/threatSubmission/emailThreatSubmissionPolicies
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Не поддерживается.

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код `200 OK` отклика и коллекцию объектов [emailThreatSubmissionPolicy](../resources/security-emailthreatsubmissionpolicy.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "list_emailthreatsubmissionpolicy"
}
-->
``` http
GET https://graph.microsoft.com/beta/security/threatSubmission/emailThreatSubmissionPolicies
```


### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.security.emailThreatSubmissionPolicy)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.security.emailThreatSubmissionPolicy",
      "id": "3df67ecc-11b4-b5b4-9bae-b0729940b3d1",
      "isReportToMicrosoftEnabled": "Boolean",
      "isReportToCustomizedEmailAddressEnabled": "Boolean",
      "isAskMeEnabledForUsers": "Boolean",
      "isAlwaysReportEnabledForUsers": "Boolean",
      "isNeverReportEnabledForUsers": "Boolean",
      "isCustomizedMessageEnabledForPhishing": "Boolean",
      "isCustomizedMessageEnabled": "Boolean",
      "customizedReportRecipientEmailAddress": "String",
      "isReviewEmailNotificationEnabled": "Boolean",
      "isCustomizedNotificationSenderEnabled": "Boolean",
      "isOrganizationBrandingEnabled": "Boolean",
      "customizedNotificationSenderEmailAddress": "String",
      "isReportFromQuarantineEnabled": "Boolean"
    }
  ]
}
```

