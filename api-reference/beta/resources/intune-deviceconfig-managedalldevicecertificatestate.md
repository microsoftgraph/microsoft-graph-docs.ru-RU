---
title: Тип ресурса Манажедаллдевицецертификатестате
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7e307c28e295282c7d6c6572a90bf6a8f5ae1746
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2019
ms.locfileid: "35741518"
---
# <a name="managedalldevicecertificatestate-resource-type"></a>Тип ресурса Манажедаллдевицецертификатестате

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Манажедаллдевицецертификатестатес](../api/intune-deviceconfig-managedalldevicecertificatestate-list.md)|Коллекция [манажедаллдевицецертификатестате](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)|Список свойств и связей объектов [манажедаллдевицецертификатестате](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) .|
|[Получение Манажедаллдевицецертификатестате](../api/intune-deviceconfig-managedalldevicecertificatestate-get.md)|[Манажедаллдевицецертификатестате](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)|Чтение свойств и связей объекта [манажедаллдевицецертификатестате](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) .|
|[Создание Манажедаллдевицецертификатестате](../api/intune-deviceconfig-managedalldevicecertificatestate-create.md)|[Манажедаллдевицецертификатестате](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)|Создание нового объекта [манажедаллдевицецертификатестате](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) .|
|[Удаление Манажедаллдевицецертификатестате](../api/intune-deviceconfig-managedalldevicecertificatestate-delete.md)|Нет|Удаляет объект [манажедаллдевицецертификатестате](../resources/intune-deviceconfig-managedalldevicecertificatestate.md).|
|[Обновление Манажедаллдевицецертификатестате](../api/intune-deviceconfig-managedalldevicecertificatestate-update.md)|[Манажедаллдевицецертификатестате](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)|Обновление свойств объекта [манажедаллдевицецертификатестате](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта.|
|Цертификатеревокестатус|[Цертификатеревокатионстатус](../resources/intune-deviceconfig-certificaterevocationstatus.md)|Отзыв состояния. Возможные значения: `none`, `pending`, `issued`, `failed`, `revoked`.|
|Манажеддевицедисплайнаме|String|Отображаемое имя устройства|
|userPrincipalName|String|Имя субъекта-пользователя|
|Цертификатикспиратиондатетиме|DateTimeOffset|Дата окончания срока действия сертификата|
|Цертификатеиссуернаме|String|Издатель|
|certificateThumbprint|String|Отпечаток|
|Цертификатесериалнумбер|String|Серийный номер|
|Цертификатесубжектнаме|String|Имя субъекта сертификата|
|Цертификатекэйусажес|Int32|Использование ключа|
|Цертификатикстендедкэйусажес|String|Расширенное использование ключа|
|Цертификатеиссуанцедатетиме|DateTimeOffset|Дата выпуска|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAllDeviceCertificateState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAllDeviceCertificateState",
  "id": "String (identifier)",
  "certificateRevokeStatus": "String",
  "managedDeviceDisplayName": "String",
  "userPrincipalName": "String",
  "certificateExpirationDateTime": "String (timestamp)",
  "certificateIssuerName": "String",
  "certificateThumbprint": "String",
  "certificateSerialNumber": "String",
  "certificateSubjectName": "String",
  "certificateKeyUsages": 1024,
  "certificateExtendedKeyUsages": "String",
  "certificateIssuanceDateTime": "String (timestamp)"
}
```





