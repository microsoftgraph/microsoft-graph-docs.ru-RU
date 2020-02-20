---
title: Тип ресурса Пфксусерцертификате
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e89c76b7fa429fad828f0b463f5b2ac6ff626685
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/20/2020
ms.locfileid: "42163565"
---
# <a name="pfxusercertificate-resource-type"></a>Тип ресурса Пфксусерцертификате

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
|tenantId|GUID|Пока не задокументировано.|
|userId|GUID|Пока не задокументировано.|
|отпечаток|String|Пока не задокументировано.|
|усерупн|String|Пока не задокументировано.|
|енкриптедпфксблоб|String|Пока не задокументировано.|
|енкриптедпфкспассворд|String|Пока не задокументировано.|
|цертстартдате|DateTimeOffset|Пока не задокументировано.|
|цертекспиратиондате|DateTimeOffset|Пока не задокументировано.|
|providerName|String|Пока не задокументировано.|
|енкриптионкэйнаме|String|Пока не задокументировано.|
|паддингсчеме|Int32|Пока нет описания|
|status|Int32|Пока нет описания|
|intendedPurpose|Int32|Пока нет описания|
|createdTime|DateTimeOffset|Пока не задокументировано.|
|isDeleted|Boolean|Пока не задокументировано|
|lastModifiedTime|DateTimeOffset|Пока не задокументировано.|
|eTag|String|Пока не задокументировано.|

## <a name="relationships"></a>Отношения
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



