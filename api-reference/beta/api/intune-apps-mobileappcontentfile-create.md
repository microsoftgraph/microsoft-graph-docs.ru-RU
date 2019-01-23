---
title: Создание объекта mobileAppContentFile
description: Создание объекта mobileAppContentFile.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c815cfcb272e0eb79465d81702e158934ec8c42a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394245"
---
# <a name="create-mobileappcontentfile"></a>Создание объекта mobileAppContentFile

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создание объекта [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).

## <a name="prerequisites"></a>Предварительные условия
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).

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
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
```

## <a name="request-headers"></a>Заголовки запросов
|Заголовок|Значение|
|:---|:---|
|Authorization|Требуется Bearer &lt;маркер&gt;
|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта mobileAppContentFile в формате JSON.

В таблице ниже приведены свойства, которые необходимо указывать при создании объекта mobileAppContentFile.

|Свойство|Тип|Описание|
|:---|:---|:---|
|azureStorageUri|String|URI службы хранилища Azure.|
|isCommitted|Boolean|Значение, указывающее, является ли файл подтвержденным.|
|id|String|Идентификатор файла.|
|createdDateTime|DateTimeOffset|Время создания файла.|
|name|String|Имя файла.|
|size|Int64|Размер файла до шифрования.|
|sizeEncrypted|Int64|Размер файла после шифрования.|
|azureStorageUriExpirationDateTime|DateTimeOffset|Время, когда заканчивается срок действия URI для службы хранилища Azure.|
|manifest|Binary|Данные манифеста.|
|uploadState|[mobileAppContentFileUploadState](../resources/intune-apps-mobileappcontentfileuploadstate.md)|Состояние текущего запроса на отправку. Возможные значения: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.|
|isFrameworkFile|Логический|Значение, указывающее, является ли файл файлом framework.|
|isDependency|Логический|Является ли содержимое файла зависимостей для основного содержимого файла.|



## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
Content-type: application/json
Content-length: 395

{
  "@odata.type": "#microsoft.graph.mobileAppContentFile",
  "azureStorageUri": "Azure Storage Uri value",
  "isCommitted": true,
  "name": "Name value",
  "size": 4,
  "sizeEncrypted": 13,
  "azureStorageUriExpirationDateTime": "2017-01-01T00:00:08.4940464-08:00",
  "manifest": "bWFuaWZlc3Q=",
  "uploadState": "transientError",
  "isFrameworkFile": true,
  "isDependency": true
}
```

### <a name="response"></a>Отклик
Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 503

{
  "@odata.type": "#microsoft.graph.mobileAppContentFile",
  "azureStorageUri": "Azure Storage Uri value",
  "isCommitted": true,
  "id": "eab2e29b-e29b-eab2-9be2-b2ea9be2b2ea",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "name": "Name value",
  "size": 4,
  "sizeEncrypted": 13,
  "azureStorageUriExpirationDateTime": "2017-01-01T00:00:08.4940464-08:00",
  "manifest": "bWFuaWZlc3Q=",
  "uploadState": "transientError",
  "isFrameworkFile": true,
  "isDependency": true
}
```




