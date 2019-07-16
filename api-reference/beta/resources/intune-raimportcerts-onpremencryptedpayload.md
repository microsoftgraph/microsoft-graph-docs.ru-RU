---
title: Тип ресурса Онпременкриптедпайлоад
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 30f0abc0c25fefd957cd9b40a0a4ae5e0f6ad953
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2019
ms.locfileid: "35741514"
---
# <a name="onpremencryptedpayload-resource-type"></a>Тип ресурса Онпременкриптедпайлоад

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Онпременкриптедпайлоадс](../api/intune-raimportcerts-onpremencryptedpayload-list.md)|Коллекция [онпременкриптедпайлоад](../resources/intune-raimportcerts-onpremencryptedpayload.md)|Список свойств и связей объектов [онпременкриптедпайлоад](../resources/intune-raimportcerts-onpremencryptedpayload.md) .|
|[Получение Онпременкриптедпайлоад](../api/intune-raimportcerts-onpremencryptedpayload-get.md)|[Онпременкриптедпайлоад](../resources/intune-raimportcerts-onpremencryptedpayload.md)|Чтение свойств и связей объекта [онпременкриптедпайлоад](../resources/intune-raimportcerts-onpremencryptedpayload.md) .|
|[Создание Онпременкриптедпайлоад](../api/intune-raimportcerts-onpremencryptedpayload-create.md)|[Онпременкриптедпайлоад](../resources/intune-raimportcerts-onpremencryptedpayload.md)|Создание нового объекта [онпременкриптедпайлоад](../resources/intune-raimportcerts-onpremencryptedpayload.md) .|
|[Удаление Онпременкриптедпайлоад](../api/intune-raimportcerts-onpremencryptedpayload-delete.md)|Нет|Удаляет объект [онпременкриптедпайлоад](../resources/intune-raimportcerts-onpremencryptedpayload.md).|
|[Обновление Онпременкриптедпайлоад](../api/intune-raimportcerts-onpremencryptedpayload-update.md)|[Онпременкриптедпайлоад](../resources/intune-raimportcerts-onpremencryptedpayload.md)|Обновление свойств объекта [онпременкриптедпайлоад](../resources/intune-raimportcerts-onpremencryptedpayload.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|tenantId|GUID|Пока не задокументировано.|
|userId|GUID|Пока не задокументировано.|
|deviceId|Guid|Пока не задокументировано.|
|Пайлоадид|GUID|Пока не задокументировано.|
|Девицекэйсумбпринт|String|Пока не задокументировано.|
|cert1PayloadUUID|String|Пока не задокументировано.|
|cert2PayloadUUID|String|Пока не задокументировано.|
|cert3PayloadUUID|String|Пока не задокументировано.|
|Плисттемплате|String|Пока не задокументировано.|
|Енкриптедблоб|Binary|Пока не задокументировано.|
|Пайлоадверсион|Int32|Пока нет описания|
|status|Int32|Пока нет описания|
|createdTime|DateTimeOffset|Пока не задокументировано.|
|lastModifiedTime|DateTimeOffset|Пока не задокументировано.|
|eTag|String|Пока не задокументировано.|
|isDeleted|Boolean|Пока не задокументировано|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.onPremEncryptedPayload"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.onPremEncryptedPayload",
  "tenantId": "Guid",
  "userId": "Guid",
  "deviceId": "Guid",
  "payloadId": "Guid",
  "deviceKeyThumbprint": "String",
  "cert1PayloadUUID": "String",
  "cert2PayloadUUID": "String",
  "cert3PayloadUUID": "String",
  "plistTemplate": "String",
  "encryptedBlob": "binary",
  "payloadVersion": 1024,
  "status": 1024,
  "createdTime": "String (timestamp)",
  "lastModifiedTime": "String (timestamp)",
  "eTag": "String",
  "isDeleted": true
}
```





