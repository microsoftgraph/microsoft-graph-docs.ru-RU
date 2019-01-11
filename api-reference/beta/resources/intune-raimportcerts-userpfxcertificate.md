---
title: Тип ресурса userPFXCertificate
description: Объект, инкапсулирующий все сведения, необходимые для пользователя PFX сертификатов.
localization_priority: Normal
ms.openlocfilehash: 87516c48e53c8117c9efa119fb6cab62844e6b68
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809998"
---
# <a name="userpfxcertificate-resource-type"></a>Тип ресурса userPFXCertificate

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Объект, инкапсулирующий все сведения, необходимые для пользователя PFX сертификатов.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список userPFXCertificates](../api/intune-raimportcerts-userpfxcertificate-list.md)|[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) коллекции|Свойства списка и связей объектов [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) .|
|[Получение userPFXCertificate](../api/intune-raimportcerts-userpfxcertificate-get.md)|[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)|Чтение свойства и связи объекта [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) .|
|[Создание userPFXCertificate](../api/intune-raimportcerts-userpfxcertificate-create.md)|[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)|Создание нового объекта [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) .|
|[Удаление userPFXCertificate](../api/intune-raimportcerts-userpfxcertificate-delete.md)|Нет|Удаляет [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md).|
|[Обновление userPFXCertificate](../api/intune-raimportcerts-userpfxcertificate-update.md)|[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)|Обновление свойства объекта [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор для сертификата PFX.|
|отпечаток|Строка|Отпечаток сертификата, PFX SHA-1.|
|intendedPurpose|[userPfxIntendedPurpose](../resources/intune-raimportcerts-userpfxintendedpurpose.md)|Сертификата своей целью с точки зрения развертывания. Возможные значения: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.|
|userPrincipalName|Строка|Имя участника-пользователя сертификата PFX.|
|startDateTime|DateTimeOffset|Дата и время начала действия сертификата.|
|expirationDateTime|DateTimeOffset|Его допустимость Дата и время окончания.|
|providerName|Строка|Поставщик криптографии для шифрования в этом больших двоичных объектов.|
|keyName|Строка|Имя ключа (в рамках поставщика) используется для шифрования больших двоичных объектов.|
|paddingScheme|[userPfxPaddingScheme](../resources/intune-raimportcerts-userpfxpaddingscheme.md)|Заполнение схемы, используемый поставщиком во время шифрования и расшифровки. Возможные значения: `none`, `pkcs1`, `oaepSha1`, `oaepSha256`, `oaepSha384`, `oaepSha512`.|
|encryptedPfxBlob|Binary|Зашифрованные больших двоичных объектов PFX.|
|encryptedPfxPassword|Строка|Зашифрованный пароль PFX.|
|createdDateTime|DateTimeOffset|Дата и время при импорте сертификата PFX.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения этого сертификата PFX.|

## <a name="relationships"></a>Связи
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





