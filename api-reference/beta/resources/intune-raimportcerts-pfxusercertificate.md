---
title: Тип ресурса pfxUserCertificate
description: Пока не задокументировано.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2d1b7482da130a0c5208aa3e0b36315be0a3bd98
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59080676"
---
# <a name="pfxusercertificate-resource-type"></a>Тип ресурса pfxUserCertificate

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список pfxUserCertificates](../api/intune-raimportcerts-pfxusercertificate-list.md)|[Коллекция pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md)|Список свойств и связей объектов [pfxUserCertificate.](../resources/intune-raimportcerts-pfxusercertificate.md)|
|[Get pfxUserCertificate](../api/intune-raimportcerts-pfxusercertificate-get.md)|[pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md)|Чтение свойств и связей объекта [pfxUserCertificate.](../resources/intune-raimportcerts-pfxusercertificate.md)|
|[Создание pfxUserCertificate](../api/intune-raimportcerts-pfxusercertificate-create.md)|[pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md)|Создайте новый [объект pfxUserCertificate.](../resources/intune-raimportcerts-pfxusercertificate.md)|
|[Удаление pfxUserCertificate](../api/intune-raimportcerts-pfxusercertificate-delete.md)|Нет|Удаляет [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md).|
|[Обновление pfxUserCertificate](../api/intune-raimportcerts-pfxusercertificate-update.md)|[pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md)|Обновление свойств объекта [pfxUserCertificate.](../resources/intune-raimportcerts-pfxusercertificate.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|tenantId|Guid|Пока не задокументировано.|
|userId|Guid|Пока не задокументировано.|
|отпечатки пальцев|String|Пока не задокументировано.|
|userUpn|String|Пока не задокументировано.|
|зашифрованныйPfxBlob|String|Пока не задокументировано.|
|зашифрованныйPfxPassword|String|Пока не задокументировано.|
|certStartDate|DateTimeOffset|Пока не задокументировано.|
|certExpirationDate|DateTimeOffset|Пока не задокументировано.|
|providerName|String|Пока не задокументировано.|
|encryptionKeyName|String|Пока не задокументировано.|
|paddingScheme|Int32|Пока не задокументировано.|
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



