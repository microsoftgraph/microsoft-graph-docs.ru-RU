---
title: Создание enterpriseCodeSigningCertificate
description: Создание нового объекта enterpriseCodeSigningCertificate.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 302c10d1e0fbc5e182180a32ad96d614555d1d04
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956194"
---
# <a name="create-enterprisecodesigningcertificate"></a>Создание enterpriseCodeSigningCertificate

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Создание нового объекта [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) .
## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementApps.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/enterpriseCodeSigningCertificates
```

## <a name="request-headers"></a>Заголовки запросов
|Заголовок|Значение|
|:---|:---|
|Authorization|Требуется Bearer &lt;маркер&gt;
|
|Accept|application/json|

## <a name="request-body"></a>Тело запроса
В тексте запроса укажите представление JSON для объекта enterpriseCodeSigningCertificate.

В следующей таблице показаны свойства, которые необходимы для создания enterpriseCodeSigningCertificate.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|content|Binary|Сертификат подписи кода Enterprise Windows в формате необработанные данные.|
|status|[certificateStatus](../resources/intune-apps-certificatestatus.md)|Состояние сертификата подготовить к работе или не подготовлен. Возможные значения: `notProvisioned`, `provisioned`.|
|subjectName|String|Имя субъекта для сертификата.|
|subject|Строка|Значения субъектов для сертификата.|
|Имя поставщика|Строка|Имя поставщика для сертификата.|
|издателя|Строка|Значение издателя сертификата.|
|expirationDateTime|DateTimeOffset|Срок действия сертификата.|
|uploadDateTime|DateTimeOffset|Дата время подписывания кода сертификата при его загрузке.|



## <a name="response"></a>Ответ
Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) в теле ответа.

## <a name="example"></a>Пример
### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/enterpriseCodeSigningCertificates
Content-type: application/json
Content-length: 390

{
  "@odata.type": "#microsoft.graph.enterpriseCodeSigningCertificate",
  "content": "Y29udGVudA==",
  "status": "provisioned",
  "subjectName": "Subject Name value",
  "subject": "Subject value",
  "issuerName": "Issuer Name value",
  "issuer": "Issuer value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "uploadDateTime": "2016-12-31T23:58:46.5747426-08:00"
}
```

### <a name="response"></a>Ответ
Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 439

{
  "@odata.type": "#microsoft.graph.enterpriseCodeSigningCertificate",
  "id": "b20d3703-3703-b20d-0337-0db203370db2",
  "content": "Y29udGVudA==",
  "status": "provisioned",
  "subjectName": "Subject Name value",
  "subject": "Subject value",
  "issuerName": "Issuer Name value",
  "issuer": "Issuer value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "uploadDateTime": "2016-12-31T23:58:46.5747426-08:00"
}
```





