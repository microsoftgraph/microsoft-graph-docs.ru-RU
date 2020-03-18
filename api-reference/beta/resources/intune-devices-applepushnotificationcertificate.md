---
title: Тип ресурса applePushNotificationCertificate
description: Сертификат push-уведомлений Apple
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 63e49aa6dfe5def2e505c7b2bf8a995c72df27c4
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42785163"
---
# <a name="applepushnotificationcertificate-resource-type"></a>Тип ресурса applePushNotificationCertificate

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сертификат push-уведомлений Apple

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение объекта applePushNotificationCertificate](../api/intune-devices-applepushnotificationcertificate-get.md)|[applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md)|Чтение свойств и связей объекта [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).|
|[Обновление объекта applePushNotificationCertificate](../api/intune-devices-applepushnotificationcertificate-update.md)|[applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md)|Обновление свойств объекта [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).|
|[Функция downloadApplePushNotificationCertificateSigningRequest](../api/intune-devices-applepushnotificationcertificate-downloadapplepushnotificationcertificatesigningrequest.md)|String|Скачивание запроса на подпись сертификата для push-уведомлений Apple|
|[действие Женератеапплепушнотификатионцертификатесигнингрекуест](../api/intune-devices-applepushnotificationcertificate-generateapplepushnotificationcertificatesigningrequest.md)|String|Скачивание запроса на подпись сертификата для push-уведомлений Apple|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор сертификата|
|appleIdentifier|String|Идентификатор Apple Id учетной записи, используемой для создания MDM Push Certificate.|
|topicIdentifier|String|Идентификатор темы.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения сертификата push-уведомлений Apple.|
|expirationDateTime|DateTimeOffset|Дата и время окончания срока действия для сертификата push-уведомлений Apple.|
|цертификатеуплоадстатус|String|Состояние отправки сертификата.|
|цертификатеуплоадфаилуререасон|String|Причина сбоя отправки сертификата.|
|цертификатесериалнумбер|String|Серийный номер сертификата. Это свойство доступно только для чтения.|
|certificate|String|Н/Д|

## <a name="relationships"></a>Связи
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
  "certificateUploadStatus": "String",
  "certificateUploadFailureReason": "String",
  "certificateSerialNumber": "String",
  "certificate": "String"
}
```



