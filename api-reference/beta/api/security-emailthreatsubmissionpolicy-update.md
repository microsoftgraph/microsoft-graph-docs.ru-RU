---
title: Обновление emailThreatSubmissionPolicy
description: Обновление свойств объекта emailThreatSubmissionPolicy.
author: caigen
ms.localizationpriority: medium
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 78ceedcdc0436f8f8eb941d6f95c65a0e6d10bba
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856746"
---
# <a name="update-emailthreatsubmissionpolicy"></a>Обновление emailThreatSubmissionPolicy
Пространство имен: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств объекта [emailThreatSubmissionPolicy](../resources/security-emailthreatsubmissionpolicy.md) .

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|ThreatSubmissionPolicies.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается|
|Приложение|ThreatSubmissionPolicy.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH security/threatSubmission/emailThreatSubmissionPolicies/{emailThreatSubmissionPoliciesId}
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]

Эти свойства связаны с параметрами сообщений, о **которых сообщил пользователь**. Дополнительные сведения см. в [разделе "Параметры сообщений, сообщаемых пользователем"](/microsoft-365/security/office-365-security/user-submission.md).

| Свойство                                 | Тип    | Описание                                                                                |
|:-----------------------------------------|:--------|:-------------------------------------------------------------------------------------------|
| customizedNotificationSenderEmailAddress | Строка  | Указывает адрес электронной почты отправителя, с которого будут отправляться уведомления по электронной почте конечным пользователям, чтобы сообщить им, является ли сообщение спамом, фишингом или очисткой. Значение по умолчанию — `null`. Необязательный для создания.                   |
| customizedReportRecipientEmailAddress    | String  | Указывает место назначения, куда будут отправляться сообщения от конечных пользователей, когда они сообщают что-то как фишинговое, нежелательное или не нежелательное. Значение по умолчанию — `null`. Необязательный для создания. |
| isAlwaysReportEnabledForUsers            | Логический | Указывает, могут ли конечные пользователи сообщать о сообщении как спаме, фишинге или нежелательной почте напрямую без подтверждения (всплывающего окна). Значение по умолчанию — `true`.  Необязательный для создания.          |
| isAskMeEnabledForUsers                   | Логический | Указывает, могут ли пользователи подтвердить использование всплывающего окна перед отправкой сообщений как спама, фишинга или нежелательной почты. Значение по умолчанию — `true`.  Необязательный для создания. |
| isCustomizedMessageEnabled               | Логический | Указывает, настроены ли уведомления по электронной почте, отправляемые конечным пользователям для уведомления о фишинге, спаме или нежелательной почте. Значение по умолчанию — `false`. Необязательный для создания.                  |
| isCustomizedMessageEnabledForPhishing    | Логический | Если этот параметр включен, настроенное сообщение отображается только в том случае, если сообщение электронной почты отображается как фишинговое. Значение по умолчанию — `false`. Необязательный для создания. |
| isCustomizedNotificationSenderEnabled    | Логический | Указывает, следует ли использовать набор адресов электронной почты отправителя с помощью customizedNotificationSenderEmailAddress для отправки уведомлений по электронной почте конечным пользователям. Значение по умолчанию — `false`. Необязательный для создания.               |
| isNeverReportEnabledForUsers             | Логический | Указывает, могут ли пользователи просто переместить сообщение из одной папки в другую на основе действий спама, фишинга или нежелательной почты без фактического сообщения о нем. Значение по умолчанию — `true`. Необязательный для создания.         |
| isOrganizationBrandingEnabled            | Логический | Указывает, следует ли использовать логотип фирменной символики в уведомлениях по электронной почте, отправляемых конечным пользователям. Значение по умолчанию — `false`. Необязательный для создания.        |
| isReportFromQuarantineEnabled            | Логический | Указывает, могут ли пользователи отправлять данные со страницы карантина. Значение по умолчанию — `true`. Необязательный для создания.              |
| isReportToCustomizedEmailAddressEnabled  | Логический | Указывает, следует ли отправлять сообщения электронной почты, сообщаемые конечными пользователями, в пользовательский почтовый ящик, настроенный с помощью customizedReportRecipientEmailAddress.  Значение по умолчанию — `false`. Необязательный для создания.              |
| isReportToMicrosoftEnabled               | Логический | Если этот параметр включен, сообщение электронной почты будет отправлено в корпорацию Майкрософт для анализа. Значение по умолчанию — `false`. Повторное создание.  |
| isReviewEmailNotificationEnabled         | Логический | Указывает, отправляется ли уведомление по электронной почте пользователю, который сообщил сообщение электронной почты при проверке администратором. Значение по умолчанию — `false`.. Необязательный для создания.  |



## <a name="response"></a>Отклик

При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "update_emailthreatsubmissionpolicy"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/security/threatSubmission/emailthreatSubmissionPolicies/DefaultReportSubmissionPolicy
Content-type: application/json

{
  "isReportToMicrosoftEnabled": false
}
```


### <a name="response"></a>Отклик
Ниже приведен пример отклика.

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

