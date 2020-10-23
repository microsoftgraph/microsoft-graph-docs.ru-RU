---
title: Тип ресурса Онпременкриптедпайлоад
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f384cedf189b8689a236208e884f7d91e392d2a2
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48707607"
---
# <a name="onpremencryptedpayload-resource-type"></a>Тип ресурса Онпременкриптедпайлоад

Пространство имен: microsoft.graph

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
|tenantId|Guid|Пока не задокументировано.|
|userId|Guid|Пока не задокументировано.|
|deviceId|Guid|Пока не задокументировано.|
|пайлоадид|Guid|Пока не задокументировано.|
|девицекэйсумбпринт|String|Пока не задокументировано.|
|cert1PayloadUUID|String|Пока не задокументировано.|
|cert2PayloadUUID|String|Пока не задокументировано.|
|cert3PayloadUUID|String|Пока не задокументировано.|
|плисттемплате|String|Пока не задокументировано.|
|енкриптедблоб|Binary|Пока не задокументировано.|
|пайлоадверсион|Int32|Пока не задокументировано.|
|status|Int32|Пока не задокументировано.|
|createdTime|DateTimeOffset|Пока не задокументировано.|
|lastModifiedTime|DateTimeOffset|Пока не задокументировано.|
|eTag|String|Пока не задокументировано.|
|isDeleted|Boolean|Н/Д|

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





