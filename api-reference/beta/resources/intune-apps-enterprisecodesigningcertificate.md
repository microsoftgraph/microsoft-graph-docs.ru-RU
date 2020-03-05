---
title: Тип ресурса Ентерприсекодесигнингцертификате
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e12fd1d9ce92acf8b1b50cc79e0e1ca6d80a5a5e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42493806"
---
# <a name="enterprisecodesigningcertificate-resource-type"></a>Тип ресурса Ентерприсекодесигнингцертификате

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список enterpriseCodeSigningCertificates](../api/intune-apps-enterprisecodesigningcertificate-list.md)|Коллекция [ентерприсекодесигнингцертификате](../resources/intune-apps-enterprisecodesigningcertificate.md)|Список свойств и связей объектов [ентерприсекодесигнингцертификате](../resources/intune-apps-enterprisecodesigningcertificate.md) .|
|[Получение Ентерприсекодесигнингцертификате](../api/intune-apps-enterprisecodesigningcertificate-get.md)|[enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md);|Чтение свойств и связей объекта [ентерприсекодесигнингцертификате](../resources/intune-apps-enterprisecodesigningcertificate.md) .|
|[Создание Ентерприсекодесигнингцертификате](../api/intune-apps-enterprisecodesigningcertificate-create.md)|[enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md);|Создание нового объекта [ентерприсекодесигнингцертификате](../resources/intune-apps-enterprisecodesigningcertificate.md) .|
|[Удаление Ентерприсекодесигнингцертификате](../api/intune-apps-enterprisecodesigningcertificate-delete.md)|Нет|Удаляет объект [ентерприсекодесигнингцертификате](../resources/intune-apps-enterprisecodesigningcertificate.md).|
|[Обновление Ентерприсекодесигнингцертификате](../api/intune-apps-enterprisecodesigningcertificate-update.md)|[enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md);|Обновление свойств объекта [ентерприсекодесигнингцертификате](../resources/intune-apps-enterprisecodesigningcertificate.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта.|
|содержимое|Binary|Сертификат подписи кода Windows Enterprise в формате необработанных данных.|
|status|[цертификатестатус](../resources/intune-apps-certificatestatus.md)|Состояние сертификата подготовлено или не подготовлено. Возможные значения: `notProvisioned`, `provisioned`.|
|subjectName|String|Имя субъекта для сертификата.|
|subject|String|Значение субъекта для сертификата.|
|иссуернаме|String|Имя поставщика сертификата.|
|имени|String|Значение издателя для сертификата.|
|expirationDateTime|DateTimeOffset|Дата окончания срока действия сертификата.|
|уплоаддатетиме|DateTimeOffset|Дата и время отправки сертификата соконструирования.|

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



