---
title: Тип ресурса enterpriseCodeSigningCertificate
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 84fe89d77901c330924c57937f9bb334beab979d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27945897"
---
# <a name="enterprisecodesigningcertificate-resource-type"></a>Тип ресурса enterpriseCodeSigningCertificate

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Н/Д
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список enterpriseCodeSigningCertificates](../api/intune-apps-enterprisecodesigningcertificate-list.md)|[enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) коллекции|Свойства списка и связей объектов [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) .|
|[Получение enterpriseCodeSigningCertificate](../api/intune-apps-enterprisecodesigningcertificate-get.md)|[enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md);|Чтение свойства и связи объекта [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) .|
|[Создание enterpriseCodeSigningCertificate](../api/intune-apps-enterprisecodesigningcertificate-create.md)|[enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md);|Создание нового объекта [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) .|
|[Удаление enterpriseCodeSigningCertificate](../api/intune-apps-enterprisecodesigningcertificate-delete.md)|Нет|Удаляет [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md).|
|[Обновление enterpriseCodeSigningCertificate](../api/intune-apps-enterprisecodesigningcertificate-update.md)|[enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md);|Обновление свойства объекта [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|content|Binary|Сертификат подписи кода Enterprise Windows в формате необработанные данные.|
|status|[certificateStatus](../resources/intune-apps-certificatestatus.md)|Состояние сертификата подготовить к работе или не подготовлен. Возможные значения: `notProvisioned`, `provisioned`.|
|subjectName|String|Имя субъекта для сертификата.|
|subject|String|Значения субъектов для сертификата.|
|Имя поставщика|String|Имя поставщика для сертификата.|
|издателя|String|Значение издателя сертификата.|
|expirationDateTime|DateTimeOffset|Срок действия сертификата.|
|uploadDateTime|DateTimeOffset|Дата время подписывания кода сертификата при его загрузке.|

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





