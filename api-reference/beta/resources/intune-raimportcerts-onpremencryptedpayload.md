---
title: onPremEncryptedPayload resource type
description: Пока не задокументировано.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3c03039367d2f25435cd27d470888f5c2b07fc2d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59074845"
---
# <a name="onpremencryptedpayload-resource-type"></a>onPremEncryptedPayload resource type

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список onPremEncryptedPayloads](../api/intune-raimportcerts-onpremencryptedpayload-list.md)|[onPremEncryptedPayload collection](../resources/intune-raimportcerts-onpremencryptedpayload.md)|Список свойств и связей объектов [onPremEncryptedPayload.](../resources/intune-raimportcerts-onpremencryptedpayload.md)|
|[Get onPremEncryptedPayload](../api/intune-raimportcerts-onpremencryptedpayload-get.md)|[onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md)|Чтение свойств и связей [объекта onPremEncryptedPayload.](../resources/intune-raimportcerts-onpremencryptedpayload.md)|
|[Создание onPremEncryptedPayload](../api/intune-raimportcerts-onpremencryptedpayload-create.md)|[onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md)|Создание нового [объекта onPremEncryptedPayload.](../resources/intune-raimportcerts-onpremencryptedpayload.md)|
|[Удаление наPremEncryptedPayload](../api/intune-raimportcerts-onpremencryptedpayload-delete.md)|Нет|Удаляет [onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md).|
|[Обновление onPremEncryptedPayload](../api/intune-raimportcerts-onpremencryptedpayload-update.md)|[onPremEncryptedPayload](../resources/intune-raimportcerts-onpremencryptedpayload.md)|Обновление свойств объекта [onPremEncryptedPayload.](../resources/intune-raimportcerts-onpremencryptedpayload.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|tenantId|Guid|Пока не задокументировано.|
|userId|Guid|Пока не задокументировано.|
|deviceId|Guid|Пока не задокументировано.|
|payloadId|Guid|Пока не задокументировано.|
|deviceKeyThumbprint|String|Пока не задокументировано.|
|cert1PayloadUUID|String|Пока не задокументировано.|
|cert2PayloadUUID|String|Пока не задокументировано.|
|cert3PayloadUUID|String|Пока не задокументировано.|
|plistTemplate|String|Пока не задокументировано.|
|encryptedBlob|В двоичном формате|Пока не задокументировано.|
|payloadVersion|Int32|Пока не задокументировано.|
|status|Int32|Пока не задокументировано.|
|createdTime|DateTimeOffset|Пока не задокументировано.|
|lastModifiedTime|DateTimeOffset|Пока не задокументировано.|
|eTag|String|Пока не задокументировано.|
|isDeleted|Boolean|Н/Д|

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



