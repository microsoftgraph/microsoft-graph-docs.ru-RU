---
title: Тип ресурса Ентерприсекодесигнингцертификате
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 75798ec0e66086b3dbf1425d297ed7f0a29808c0
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33950468"
---
# <a name="enterprisecodesigningcertificate-resource-type"></a>Тип ресурса Ентерприсекодесигнингцертификате

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

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
|status|[Цертификатестатус](../resources/intune-apps-certificatestatus.md)|Состояние сертификата подготовлено или не подготовлено. Возможные значения: `notProvisioned`, `provisioned`.|
|subjectName|String|Имя субъекта для сертификата.|
|subject|String|Значение субъекта для сертификата.|
|Иссуернаме|Строка|Имя поставщика сертификата.|
|имени|Строка|Значение издателя для сертификата.|
|expirationDateTime|DateTimeOffset|Дата окончания срока действия сертификата.|
|Уплоаддатетиме|DateTimeOffset|Дата и время отправки сертификата соконструирования.|

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




