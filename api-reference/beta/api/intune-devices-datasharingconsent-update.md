---
title: Обновление dataSharingConsent
description: Обновление свойства объекта dataSharingConsent.
author: tfitzmac
ms.openlocfilehash: 1d7759def9c11165fca0b646f166ac792c14369e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27317635"
---
# <a name="update-datasharingconsent"></a>Обновление dataSharingConsent

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Обновление свойства объекта [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) .
## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementServiceConfig.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/dataSharingConsents/{dataSharingConsentId}
```

## <a name="request-headers"></a>Заголовки запросов
|Заголовок|Значение|
|:---|:---|
|Авторизация|Требуется Bearer &lt;маркер&gt;
|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В тексте запроса укажите представление JSON для объекта [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) .

В следующей таблице показаны свойства, которые необходимы для создания [dataSharingConsent](../resources/intune-devices-datasharingconsent.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Разрешения общего доступа данных идентификатор|
|Отображаемое_имя_службы|String.|Отображаемое имя службы рабочих процессов|
|termsUrl|String.|TermsUrl для данных, общий доступ к согласия|
|предоставлено|Boolean.|Предоставленные состояний для данных, общий доступ к согласия|
|grantDateTime|DateTimeOffset|Были предоставлены разрешения времени для этой учетной записи|
|grantedByUpn|String.|Имя участника-пользователя, которой предоставлены разрешения для этой учетной записи|
|grantedByUserId|String.|Идентификатор пользователя, который предоставлены разрешения для этой учетной записи пользователя|



## <a name="response"></a>Ответ
Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) объекта в теле ответа.

## <a name="example"></a>Пример
### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/dataSharingConsents/{dataSharingConsentId}
Content-type: application/json
Content-length: 276

{
  "serviceDisplayName": "Service Display Name value",
  "termsUrl": "https://example.com/termsUrl/",
  "granted": true,
  "grantDateTime": "2016-12-31T23:59:55.7154191-08:00",
  "grantedByUpn": "Granted By Upn value",
  "grantedByUserId": "Granted By User Id value"
}
```

### <a name="response"></a>Ответ
Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 382

{
  "@odata.type": "#microsoft.graph.dataSharingConsent",
  "id": "333387f7-87f7-3333-f787-3333f7873333",
  "serviceDisplayName": "Service Display Name value",
  "termsUrl": "https://example.com/termsUrl/",
  "granted": true,
  "grantDateTime": "2016-12-31T23:59:55.7154191-08:00",
  "grantedByUpn": "Granted By Upn value",
  "grantedByUserId": "Granted By User Id value"
}
```





