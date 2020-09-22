---
title: Тип ресурса Пфксусерцертификате
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 514e3d4c858a49ab51f5c3f7565ae4ccdf64be6e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47993282"
---
# <a name="pfxusercertificate-resource-type"></a>Тип ресурса Пфксусерцертификате

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Пфксусерцертификатес](../api/intune-raimportcerts-pfxusercertificate-list.md)|Коллекция [пфксусерцертификате](../resources/intune-raimportcerts-pfxusercertificate.md)|Список свойств и связей объектов [пфксусерцертификате](../resources/intune-raimportcerts-pfxusercertificate.md) .|
|[Получение Пфксусерцертификате](../api/intune-raimportcerts-pfxusercertificate-get.md)|[пфксусерцертификате](../resources/intune-raimportcerts-pfxusercertificate.md)|Чтение свойств и связей объекта [пфксусерцертификате](../resources/intune-raimportcerts-pfxusercertificate.md) .|
|[Создание Пфксусерцертификате](../api/intune-raimportcerts-pfxusercertificate-create.md)|[пфксусерцертификате](../resources/intune-raimportcerts-pfxusercertificate.md)|Создание нового объекта [пфксусерцертификате](../resources/intune-raimportcerts-pfxusercertificate.md) .|
|[Удаление Пфксусерцертификате](../api/intune-raimportcerts-pfxusercertificate-delete.md)|Нет|Удаляет объект [пфксусерцертификате](../resources/intune-raimportcerts-pfxusercertificate.md).|
|[Обновление Пфксусерцертификате](../api/intune-raimportcerts-pfxusercertificate-update.md)|[пфксусерцертификате](../resources/intune-raimportcerts-pfxusercertificate.md)|Обновление свойств объекта [пфксусерцертификате](../resources/intune-raimportcerts-pfxusercertificate.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|tenantId|Guid|Пока не задокументировано.|
|userId|Guid|Пока не задокументировано.|
|отпечаток|String|Пока не задокументировано.|
|усерупн|String|Пока не задокументировано.|
|енкриптедпфксблоб|String|Пока не задокументировано.|
|енкриптедпфкспассворд|String|Пока не задокументировано.|
|цертстартдате|DateTimeOffset|Пока не задокументировано.|
|цертекспиратиондате|DateTimeOffset|Пока не задокументировано.|
|providerName|String|Пока не задокументировано.|
|енкриптионкэйнаме|String|Пока не задокументировано.|
|паддингсчеме|Int32|Пока не задокументировано.|
|status|Int32|Пока не задокументировано.|
|intendedPurpose|Int32|Пока не задокументировано.|
|createdTime|DateTimeOffset|Пока не задокументировано.|
|isDeleted|Boolean|Н/Д|
|lastModifiedTime|DateTimeOffset|Пока не задокументировано.|
|eTag|String|Н/Д|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.pfxUserCertificate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.pfxUserCertificate",
  "tenantId": "Guid",
  "userId": "Guid",
  "thumbprint": "String",
  "userUpn": "String",
  "encryptedPfxBlob": "String",
  "encryptedPfxPassword": "String",
  "certStartDate": "String (timestamp)",
  "certExpirationDate": "String (timestamp)",
  "providerName": "String",
  "encryptionKeyName": "String",
  "paddingScheme": 1024,
  "status": 1024,
  "intendedPurpose": 1024,
  "createdTime": "String (timestamp)",
  "isDeleted": true,
  "lastModifiedTime": "String (timestamp)",
  "eTag": "String"
}
```






