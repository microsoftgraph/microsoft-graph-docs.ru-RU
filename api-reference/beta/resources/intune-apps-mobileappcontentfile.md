---
title: Тип ресурса mobileAppContentFile
description: Содержит свойства для одного файла установщика, связанного с заданной версией mobileAppContent.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5e9f28ea036bbe73fae8e9e59d8d63ea8916f15d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425682"
---
# <a name="mobileappcontentfile-resource-type"></a>Тип ресурса mobileAppContentFile

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

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
|isFrameworkFile|Логический|Значение, указывающее, является ли файл файлом framework.|
|isDependency|Логический|Является ли содержимое файла зависимостей для основного содержимого файла.|

## <a name="relationships"></a>Отношения
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
  "uploadState": "String",
  "isFrameworkFile": true,
  "isDependency": true
}
```




