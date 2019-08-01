---
title: Тип ресурса applePushNotificationCertificate
description: Сертификат push-уведомлений Apple
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2c56f78a596d08037ca68a96bf9cc5aca5fbf148
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36027505"
---
# <a name="applepushnotificationcertificate-resource-type"></a>Тип ресурса applePushNotificationCertificate

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сертификат push-уведомлений Apple

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение объекта applePushNotificationCertificate](../api/intune-devices-applepushnotificationcertificate-get.md)|[applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md)|Чтение свойств и связей объекта [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).|
|[Обновление объекта applePushNotificationCertificate](../api/intune-devices-applepushnotificationcertificate-update.md)|[applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md)|Обновление свойств объекта [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).|
|[Функция downloadApplePushNotificationCertificateSigningRequest](../api/intune-devices-applepushnotificationcertificate-downloadapplepushnotificationcertificatesigningrequest.md)|String|Скачивание запроса на подпись сертификата для push-уведомлений Apple|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор сертификата|
|appleIdentifier|String|Идентификатор Apple Id учетной записи, используемой для создания MDM Push Certificate.|
|topicIdentifier|String|Идентификатор темы.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения сертификата push-уведомлений Apple.|
|expirationDateTime|DateTimeOffset|Дата и время окончания срока действия для сертификата push-уведомлений Apple.|
|certificate|String|Н/Д|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.applePushNotificationCertificate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.applePushNotificationCertificate",
  "id": "String (identifier)",
  "appleIdentifier": "String",
  "topicIdentifier": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)",
  "certificate": "String"
}
```



