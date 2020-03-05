---
title: Тип ресурса Онпременкриптедпайлоад
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 08d5f3102bb2c748d24235290a8f75abe8408334
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527599"
---
# <a name="onpremencryptedpayload-resource-type"></a>Тип ресурса Онпременкриптедпайлоад

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Онпременкриптедпайлоадс](../api/intune-raimportcerts-onpremencryptedpayload-list.md)|Коллекция [онпременкриптедпайлоад](../resources/intune-raimportcerts-onpremencryptedpayload.md)|Список свойств и связей объектов [онпременкриптедпайлоад](../resources/intune-raimportcerts-onpremencryptedpayload.md) .|
|[Получение Онпременкриптедпайлоад](../api/intune-raimportcerts-onpremencryptedpayload-get.md)|[онпременкриптедпайлоад](../resources/intune-raimportcerts-onpremencryptedpayload.md)|Чтение свойств и связей объекта [онпременкриптедпайлоад](../resources/intune-raimportcerts-onpremencryptedpayload.md) .|
|[Создание Онпременкриптедпайлоад](../api/intune-raimportcerts-onpremencryptedpayload-create.md)|[онпременкриптедпайлоад](../resources/intune-raimportcerts-onpremencryptedpayload.md)|Создание нового объекта [онпременкриптедпайлоад](../resources/intune-raimportcerts-onpremencryptedpayload.md) .|
|[Удаление Онпременкриптедпайлоад](../api/intune-raimportcerts-onpremencryptedpayload-delete.md)|Нет|Удаляет объект [онпременкриптедпайлоад](../resources/intune-raimportcerts-onpremencryptedpayload.md).|
|[Обновление Онпременкриптедпайлоад](../api/intune-raimportcerts-onpremencryptedpayload-update.md)|[онпременкриптедпайлоад](../resources/intune-raimportcerts-onpremencryptedpayload.md)|Обновление свойств объекта [онпременкриптедпайлоад](../resources/intune-raimportcerts-onpremencryptedpayload.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|tenantId|GUID|Пока не задокументировано.|
|userId|GUID|Пока не задокументировано.|
|deviceId|Guid|Пока не задокументировано.|
|пайлоадид|GUID|Пока не задокументировано.|
|девицекэйсумбпринт|String|Пока не задокументировано.|
|cert1PayloadUUID|String|Пока не задокументировано.|
|cert2PayloadUUID|String|Пока не задокументировано.|
|cert3PayloadUUID|String|Пока не задокументировано.|
|плисттемплате|String|Пока не задокументировано.|
|енкриптедблоб|Binary|Пока не задокументировано.|
|пайлоадверсион|Int32|Пока нет описания|
|status|Int32|Пока нет описания|
|createdTime|DateTimeOffset|Пока не задокументировано.|
|lastModifiedTime|DateTimeOffset|Пока не задокументировано.|
|eTag|String|Пока не задокументировано.|
|isDeleted|Boolean|Пока не задокументировано|

## <a name="relationships"></a>Связи
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



