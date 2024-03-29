---
title: тип ресурса userPFXCertificate
description: Объект, инкапсулирует всю информацию, необходимую для сертификатов PFX пользователя.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e293370df72fee56ffe94cfdfac8b869bc73be1f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59080662"
---
# <a name="userpfxcertificate-resource-type"></a>тип ресурса userPFXCertificate

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект, инкапсулирует всю информацию, необходимую для сертификатов PFX пользователя.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список пользователейPFXCertificates](../api/intune-raimportcerts-userpfxcertificate-list.md)|[коллекция userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)|Список свойств и связей [объектов userPFXCertificate.](../resources/intune-raimportcerts-userpfxcertificate.md)|
|[Get userPFXCertificate](../api/intune-raimportcerts-userpfxcertificate-get.md)|[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)|Чтение свойств и связей [объекта userPFXCertificate.](../resources/intune-raimportcerts-userpfxcertificate.md)|
|[Создание userPFXCertificate](../api/intune-raimportcerts-userpfxcertificate-create.md)|[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)|Создайте новый [объект userPFXCertificate.](../resources/intune-raimportcerts-userpfxcertificate.md)|
|[Удаление userPFXCertificate](../api/intune-raimportcerts-userpfxcertificate-delete.md)|Нет|Удаляет [пользователяPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md).|
|[Обновление userPFXCertificate](../api/intune-raimportcerts-userpfxcertificate-update.md)|[userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md)|Обновление свойств объекта [userPFXCertificate.](../resources/intune-raimportcerts-userpfxcertificate.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для сертификата PFX.|
|отпечатки пальцев|String|Отпечатки sha-1 сертификата PFX.|
|intendedPurpose|[userPfxIntendedPurpose](../resources/intune-raimportcerts-userpfxintendedpurpose.md)|Предназначение сертификата с точки зрения развертывания. Возможные значения: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.|
|userPrincipalName|String|Имя пользователя сертификата PFX.|
|startDateTime|DateTimeOffset|Дата начала действия сертификата.|
|expirationDateTime|DateTimeOffset|Срок действия сертификата.|
|providerName|String|Поставщик криптографии, используемый для шифрования этого blob.|
|keyName|String|Имя ключа (в пределах поставщика), используемого для шифрования blob.|
|paddingScheme|[userPfxPaddingScheme](../resources/intune-raimportcerts-userpfxpaddingscheme.md)|Схема заполнения, используемая поставщиком при шифровании и расшифровке. Возможные значения: `none`, `pkcs1`, `oaepSha1`, `oaepSha256`, `oaepSha384`, `oaepSha512`.|
|зашифрованныйPfxBlob|В двоичном формате|Зашифрованный BLOB PFX.|
|зашифрованныйPfxPassword|String|Зашифрованный пароль PFX.|
|createdDateTime|DateTimeOffset|Дата и время импорта этого сертификата PFX.|
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



