---
title: тип ресурса enterpriseCodeSigningCertificate
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cf469c4d1aa86a3acbc5dba823b671c93146258d
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58783003"
---
# <a name="enterprisecodesigningcertificate-resource-type"></a>тип ресурса enterpriseCodeSigningCertificate

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список enterpriseCodeSigningCertificates](../api/intune-apps-enterprisecodesigningcertificate-list.md)|[коллекция enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md)|Список свойств и связей [объектов enterpriseCodeSigningCertificate.](../resources/intune-apps-enterprisecodesigningcertificate.md)|
|[Get enterpriseCodeSigningCertificate](../api/intune-apps-enterprisecodesigningcertificate-get.md)|[enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md);|Чтение свойств и связей [объекта enterpriseCodeSigningCertificate.](../resources/intune-apps-enterprisecodesigningcertificate.md)|
|[Создание enterpriseCodeSigningCertificate](../api/intune-apps-enterprisecodesigningcertificate-create.md)|[enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md);|Создание нового [объекта enterpriseCodeSigningCertificate.](../resources/intune-apps-enterprisecodesigningcertificate.md)|
|[Удаление enterpriseCodeSigningCertificate](../api/intune-apps-enterprisecodesigningcertificate-delete.md)|Нет|Удаляет [корпоративнуюCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md).|
|[Обновление enterpriseCodeSigningCertificate](../api/intune-apps-enterprisecodesigningcertificate-update.md)|[enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md);|Обновление свойств объекта [enterpriseCodeSigningCertificate.](../resources/intune-apps-enterprisecodesigningcertificate.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта.|
|содержимое|В двоичном формате|Сертификат Windows Enterprise Code-Signing в формате необработанных данных.|
|status|[certificateStatus](../resources/intune-apps-certificatestatus.md)|Состояние сертификата, предварительное или не предварительное. Возможные значения: `notProvisioned`, `provisioned`.|
|subjectName|String|Имя субъекта для сертификата.|
|subject|String|Значение subject для сертификата.|
|issuerName|Строка|Имя эмитента для сертификата.|
|эмитент|Строка|Значение Issuer для сертификата.|
|expirationDateTime|DateTimeOffset|Срок действия сертификата.|
|uploadDateTime|DateTimeOffset|Время даты отправки сертификата CodeSigning.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.enterpriseCodeSigningCertificate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.enterpriseCodeSigningCertificate",
  "id": "String (identifier)",
  "content": "binary",
  "status": "String",
  "subjectName": "String",
  "subject": "String",
  "issuerName": "String",
  "issuer": "String",
  "expirationDateTime": "String (timestamp)",
  "uploadDateTime": "String (timestamp)"
}
```



