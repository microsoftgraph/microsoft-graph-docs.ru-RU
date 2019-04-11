---
title: Тип ресурса Усерпфксцертификате
description: Объект, инкапсулирующий все сведения, необходимые для сертификатов пользователя PFX.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 31a634c8c442cdbf53034b7d39062c1a3d0f5a01
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31789866"
---
# <a name="userpfxcertificate-resource-type"></a>Тип ресурса Усерпфксцертификате

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект, инкапсулирующий все сведения, необходимые для сертификатов пользователя PFX.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Усерпфксцертификатес](../api/intune-raimportcerts-userpfxcertificate-list.md)|Коллекция [усерпфксцертификате](../resources/intune-raimportcerts-userpfxcertificate.md)|Список свойств и связей объектов [усерпфксцертификате](../resources/intune-raimportcerts-userpfxcertificate.md) .|
|[Получение Усерпфксцертификате](../api/intune-raimportcerts-userpfxcertificate-get.md)|[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)|Чтение свойств и связей объекта [усерпфксцертификате](../resources/intune-raimportcerts-userpfxcertificate.md) .|
|[Создание Усерпфксцертификате](../api/intune-raimportcerts-userpfxcertificate-create.md)|[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)|Создание нового объекта [усерпфксцертификате](../resources/intune-raimportcerts-userpfxcertificate.md) .|
|[Удаление Усерпфксцертификате](../api/intune-raimportcerts-userpfxcertificate-delete.md)|Нет|Удаляет объект [усерпфксцертификате](../resources/intune-raimportcerts-userpfxcertificate.md).|
|[Обновление Усерпфксцертификате](../api/intune-raimportcerts-userpfxcertificate-update.md)|[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)|Обновление свойств объекта [усерпфксцертификате](../resources/intune-raimportcerts-userpfxcertificate.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор для сертификата PFX.|
|отпечаток|String|Отпечаток SHA-1 сертификата PFX.|
|intendedPurpose|[userPfxIntendedPurpose](../resources/intune-raimportcerts-userpfxintendedpurpose.md)|Сертификат, предназначенный для целей из точки зрения развертывания. Возможные значения: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.|
|userPrincipalName|String|Имя участника-пользователя сертификата PFX.|
|startDateTime|DateTimeOffset|Дата и время начала действия сертификата.|
|expirationDateTime|DateTimeOffset|Дата и время действия сертификата.|
|providerName|String|Поставщик криптографии, используемый для шифрования этого объекта BLOB.|
|keyName|String|Имя ключа (в пределах поставщика), используемого для шифрования большого двоичного объекта.|
|Паддингсчеме|[userPfxPaddingScheme](../resources/intune-raimportcerts-userpfxpaddingscheme.md)|Схема заполнения, используемая поставщиком во время шифрования и расшифровки. Возможные значения: `none`, `pkcs1`, `oaepSha1`, `oaepSha256`, `oaepSha384`, `oaepSha512`.|
|Енкриптедпфксблоб|Binary|Зашифрованный BLOB-объект PFX.|
|Енкриптедпфкспассворд|String|Зашифрованный пароль PFX.|
|createdDateTime|DateTimeOffset|Дата и время импорта этого PFX-сертификата.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения сертификата PFX.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userPFXCertificate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userPFXCertificate",
  "id": "String (identifier)",
  "thumbprint": "String",
  "intendedPurpose": "String",
  "userPrincipalName": "String",
  "startDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)",
  "providerName": "String",
  "keyName": "String",
  "paddingScheme": "String",
  "encryptedPfxBlob": "binary",
  "encryptedPfxPassword": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)"
}
```



