---
title: Тип ресурса Микрософттуннелсите
description: Объект, представляющий сайт туннеля Microsoft
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 730d0075009b605db5e132412bddfbf0f58251a6
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49302098"
---
# <a name="microsofttunnelsite-resource-type"></a>Тип ресурса Микрософттуннелсите

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект, представляющий сайт туннеля Microsoft

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Микрософттуннелситес](../api/intune-mstunnel-microsofttunnelsite-list.md)|Коллекция [микрософттуннелсите](../resources/intune-mstunnel-microsofttunnelsite.md)|Список свойств и связей объектов [микрософттуннелсите](../resources/intune-mstunnel-microsofttunnelsite.md) .|
|[Получение Микрософттуннелсите](../api/intune-mstunnel-microsofttunnelsite-get.md)|[микрософттуннелсите](../resources/intune-mstunnel-microsofttunnelsite.md)|Чтение свойств и связей объекта [микрософттуннелсите](../resources/intune-mstunnel-microsofttunnelsite.md) .|
|[Создание Микрософттуннелсите](../api/intune-mstunnel-microsofttunnelsite-create.md)|[микрософттуннелсите](../resources/intune-mstunnel-microsofttunnelsite.md)|Создание нового объекта [микрософттуннелсите](../resources/intune-mstunnel-microsofttunnelsite.md) .|
|[Удаление Микрософттуннелсите](../api/intune-mstunnel-microsofttunnelsite-delete.md)|Нет|Удаляет объект [микрософттуннелсите](../resources/intune-mstunnel-microsofttunnelsite.md).|
|[Обновление Микрософттуннелсите](../api/intune-mstunnel-microsofttunnelsite-update.md)|[микрософттуннелсите](../resources/intune-mstunnel-microsofttunnelsite.md)|Обновление свойств объекта [микрософттуннелсите](../resources/intune-mstunnel-microsofttunnelsite.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор Микрософттуннелсите|
|displayName|String|Отображаемое имя Микрософттуннелсите|
|description|String|Описание Микрософттуннелсите|
|публикаддресс|String|Имя или IP-адрес общедоступного домена Микрософттуннелсите|
|roleScopeTagIds|Коллекция строк|Список тегов областей для этого экземпляра сущности.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|микрософттуннелконфигуратион|[микрософттуннелконфигуратион](../resources/intune-mstunnel-microsofttunnelconfiguration.md)|Микрософттуннелконфигуратион, примененный к данному Микрософттуннелсите|
|микрософттуннелсерверс|Коллекция [микрософттуннелсервер](../resources/intune-mstunnel-microsofttunnelserver.md)|Список Микрософттуннелсерверс, зарегистрированных для этого Микрософттуннелсите|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.microsoftTunnelSite"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftTunnelSite",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "publicAddress": "String",
  "roleScopeTagIds": [
    "String"
  ]
}
```




