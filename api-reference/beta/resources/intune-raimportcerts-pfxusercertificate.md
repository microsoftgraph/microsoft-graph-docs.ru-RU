---
title: Тип ресурса Пфксусерцертификате
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b9f709281d4ca0711fab6d2cf9a5c8fd453ba32b
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2019
ms.locfileid: "35741524"
---
# <a name="pfxusercertificate-resource-type"></a>Тип ресурса Пфксусерцертификате

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Пфксусерцертификатес](../api/intune-raimportcerts-pfxusercertificate-list.md)|Коллекция [пфксусерцертификате](../resources/intune-raimportcerts-pfxusercertificate.md)|Список свойств и связей объектов [пфксусерцертификате](../resources/intune-raimportcerts-pfxusercertificate.md) .|
|[Получение Пфксусерцертификате](../api/intune-raimportcerts-pfxusercertificate-get.md)|[Пфксусерцертификате](../resources/intune-raimportcerts-pfxusercertificate.md)|Чтение свойств и связей объекта [пфксусерцертификате](../resources/intune-raimportcerts-pfxusercertificate.md) .|
|[Создание Пфксусерцертификате](../api/intune-raimportcerts-pfxusercertificate-create.md)|[Пфксусерцертификате](../resources/intune-raimportcerts-pfxusercertificate.md)|Создание нового объекта [пфксусерцертификате](../resources/intune-raimportcerts-pfxusercertificate.md) .|
|[Удаление Пфксусерцертификате](../api/intune-raimportcerts-pfxusercertificate-delete.md)|Нет|Удаляет объект [пфксусерцертификате](../resources/intune-raimportcerts-pfxusercertificate.md).|
|[Обновление Пфксусерцертификате](../api/intune-raimportcerts-pfxusercertificate-update.md)|[Пфксусерцертификате](../resources/intune-raimportcerts-pfxusercertificate.md)|Обновление свойств объекта [пфксусерцертификате](../resources/intune-raimportcerts-pfxusercertificate.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|tenantId|GUID|Пока не задокументировано.|
|userId|GUID|Пока не задокументировано.|
|отпечаток|String|Пока не задокументировано.|
|Усерупн|String|Пока не задокументировано.|
|Енкриптедпфксблоб|String|Пока не задокументировано.|
|Енкриптедпфкспассворд|String|Пока не задокументировано.|
|Цертстартдате|DateTimeOffset|Пока не задокументировано.|
|Цертекспиратиондате|DateTimeOffset|Пока не задокументировано.|
|providerName|String|Пока не задокументировано.|
|Енкриптионкэйнаме|String|Пока не задокументировано.|
|Паддингсчеме|Int32|Пока нет описания|
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





