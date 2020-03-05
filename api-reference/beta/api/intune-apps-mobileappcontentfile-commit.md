---
title: Действие commit
description: Подтверждает файл заданного приложения.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fae37bf00edb17657841c5f784ba686ba5172bae
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42450750"
---
# <a name="commit-action"></a>Действие commit

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Подтверждает файл заданного приложения.

## <a name="prerequisites"></a>Предварительные условия
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementApps.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|DeviceManagementApps.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}/commit
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В тело запроса добавьте параметры в формате JSON.

В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.

|Свойство|Тип|Описание|
|:---|:---|:---|
|fileEncryptionInfo|[fileEncryptionInfo](../resources/intune-apps-fileencryptioninfo.md)|Ключ параметра сведений о шифровании файлов.|



## <a name="response"></a>Отклик
В случае успешного выполнения это действие возвращает код отклика `204 No Content`.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}/commit

Content-type: application/json
Content-length: 399

{
  "fileEncryptionInfo": {
    "@odata.type": "microsoft.graph.fileEncryptionInfo",
    "encryptionKey": "ZW5jcnlwdGlvbktleQ==",
    "initializationVector": "aW5pdGlhbGl6YXRpb25WZWN0b3I=",
    "mac": "bWFj",
    "macKey": "bWFjS2V5",
    "profileIdentifier": "Profile Identifier value",
    "fileDigest": "ZmlsZURpZ2VzdA==",
    "fileDigestAlgorithm": "File Digest Algorithm value"
  }
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 204 No Content
```





