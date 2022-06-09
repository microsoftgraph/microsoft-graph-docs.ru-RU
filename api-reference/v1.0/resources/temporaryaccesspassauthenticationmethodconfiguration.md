---
title: Тип ресурса temporaryAccessPassAuthenticationMethodConfiguration
description: Представляет политику методов проверки подлинности временного прохода доступа, которая определяет параметры конфигурации и пользователей или группы, которым разрешено использовать метод проверки подлинности.
author: tilarso
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
doc_type: apiPageType
ms.openlocfilehash: 00a797efd68cefe8daf96e46a2d4b92f265bd488
ms.sourcegitcommit: 4b852b92535fba8af9b2bbd6f55dc16aced9ef7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/09/2022
ms.locfileid: "65971728"
---
# <a name="temporaryaccesspassauthenticationmethodconfiguration-resource-type"></a>Тип ресурса temporaryAccessPassAuthenticationMethodConfiguration
Пространство имен: microsoft.graph

Представляет политику методов проверки подлинности временного прохода доступа, которая определяет параметры конфигурации и пользователей или группы, которым разрешено использовать метод проверки подлинности.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Получение](../api/temporaryaccesspassauthenticationmethodconfiguration-get.md)|[temporaryaccesspassauthenticationmethodconfiguration](../resources/temporaryaccesspassauthenticationmethodconfiguration.md)|Чтение свойств и связей **временного объектаAccessPassAuthenticationMethodConfiguration** .|
|[Обновление](../api/temporaryaccesspassauthenticationmethodconfiguration-update.md)|Нет|Обновление свойств объекта **temporaryAccessPassAuthenticationMethodConfiguration** .|
|[Удаление](../api/temporaryaccesspassauthenticationmethodconfiguration-delete.md)|Нет|Возвращает объект **temporaryAccessPassAuthenticationMethodConfiguration** в конфигурацию по умолчанию.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|defaultLength|Целое|Длина по умолчанию в символах временного объектаAccessPass. Должен содержать от 8 до 48 символов.|
|defaultLifetimeInMinutes|Целое|Время существования по умолчанию в минутах для временного приложенияAccessPass. Значение может быть любым целым числом между **minimumLifetimeInMinutes** и **maximumLifetimeInMinutes**.|
|id|String|Идентификатор политики метода проверки подлинности. Наследуется от [сущности](entity.md).|
|isUsableOnce|Boolean   |Если `true`все проходы в клиенте будут ограничены однонастройным использованием. Если `false`этот параметр передается клиенту, его можно создать для одноразового использования или повторного использования.|
|minimumLifetimeInMinutes|Целое|Минимальное время существования в минутах для любого временного приложенияAccessPass, созданного в клиенте. Значение может быть в диапазоне от 10 до 43200 минут (эквивалентно 30 дням).|
|maximumLifetimeInMinutes|Целое|Максимальное время существования в минутах для любого временного приложенияAccessPass, созданного в клиенте. Значение может быть в диапазоне от 10 до 43200 минут (эквивалентно 30 дням).|
|state|authenticationMethodState|Включен ли в клиенте метод временного сквозного доступа. Возможные значения: `enabled`, `disabled`. Наследуется [от authenticationMethodConfiguration](authenticationmethodconfiguration.md). |

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|includeTargets|[Коллекция authenticationMethodTarget](../resources/authenticationmethodtarget.md)|Коллекция пользователей или групп, которым разрешено использовать метод проверки подлинности.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.temporaryAccessPassAuthenticationMethodConfiguration",
  "baseType": "microsoft.graph.authenticationMethodConfiguration",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.temporaryAccessPassAuthenticationMethodConfiguration",
  "id": "String (identifier)",
  "state": "String",
  "defaultLifetimeInMinutes": "Integer",
  "defaultLength": "Integer",
  "minimumLifetimeInMinutes": "Integer",
  "maximumLifetimeInMinutes": "Integer",
  "isUsableOnce": "Boolean",
  "includeTargets": [ { "@odata.type": "microsoft.graph.authenticationMethodTarget" } ]
}
```
