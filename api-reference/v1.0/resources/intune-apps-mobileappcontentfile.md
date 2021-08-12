---
title: Тип ресурса mobileAppContentFile
description: Содержит свойства для одного файла установщика, связанного с заданной версией mobileAppContent.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 00d05b36cb2ca06a459d7065a2f5fde6d3e993a270d1c5b61fd95aa53bde9716
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54205817"
---
# <a name="mobileappcontentfile-resource-type"></a>Тип ресурса mobileAppContentFile

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства для одного файла установщика, связанного с заданной версией mobileAppContent.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление mobileAppContentFiles](../api/intune-apps-mobileappcontentfile-list.md)|Коллекция [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)|Список свойств и связей объектов [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).|
|[Получение mobileAppContentFile](../api/intune-apps-mobileappcontentfile-get.md)|[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)|Считывание свойств и связей объекта [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).|
|[Создание mobileAppContentFile](../api/intune-apps-mobileappcontentfile-create.md)|[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)|Создание объекта [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).|
|[Удаление mobileAppContentFile](../api/intune-apps-mobileappcontentfile-delete.md)|None|Удаление экземпляра [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).|
|[Обновление mobileAppContentFile](../api/intune-apps-mobileappcontentfile-update.md)|[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)|Обновление свойств объекта [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).|
|[Действие commit](../api/intune-apps-mobileappcontentfile-commit.md)|None|Подтверждает файл заданного приложения.|
|[Действие renewUpload](../api/intune-apps-mobileappcontentfile-renewupload.md)|None|Обновляет URI SAS для отправки файла приложения.|

## <a name="properties"></a>Свойства
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

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppContentFile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppContentFile",
  "azureStorageUri": "String",
  "isCommitted": true,
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "name": "String",
  "size": 1024,
  "sizeEncrypted": 1024,
  "azureStorageUriExpirationDateTime": "String (timestamp)",
  "manifest": "binary",
  "uploadState": "String"
}
```




