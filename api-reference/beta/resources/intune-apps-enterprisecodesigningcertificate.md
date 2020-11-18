---
title: Тип ресурса Ентерприсекодесигнингцертификате
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0748b255faa5641dee9dce8c34ca460d935e68a2
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49200283"
---
# <a name="enterprisecodesigningcertificate-resource-type"></a>Тип ресурса Ентерприсекодесигнингцертификате

Пространство имен: microsoft.graph

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
|id|String|Ключ объекта.|
|содержимое|Binary|Сертификат Windows корпоративный Code-Signing в формате необработанных данных.|
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




