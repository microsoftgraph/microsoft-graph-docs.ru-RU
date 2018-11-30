---
title: Тип ресурса termsAndConditions
description: Содержимое C политик, изучите пользователям при их первая попытка возможность зачисления в Intune, а затем после изменения которой необходимо re приемки администратора. Благодаря им администраторы могут огласить условия, с которыми должен согласиться пользователь для регистрации устройств в Intune.
ms.openlocfilehash: 73a79a4e0684f04cb7c8caaff1e9ed944af7fe80
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027343"
---
# <a name="termsandconditions-resource-type"></a>Тип ресурса termsAndConditions

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Объект termsAndConditions представляет метаданные и содержимое определенной политики условий. Содержимое политик условий предоставляется пользователю при первой попытке регистрации в Intune, а после этого — при правках, которые нужно повторно принять по требованию администратора. Благодаря им администраторы могут огласить условия, с которыми должен согласиться пользователь для регистрации устройств в Intune.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов termsAndConditions](../api/intune-companyterms-termsandconditions-list.md)|Коллекция объектов [termsAndConditions](../resources/intune-companyterms-termsandconditions.md)|Список свойств и связей объектов [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).|
|[Получение объекта termsAndConditions](../api/intune-companyterms-termsandconditions-get.md)|[termsAndConditions](../resources/intune-companyterms-termsandconditions.md)|Чтение свойств и связей объекта [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).|
|[Создание объекта termsAndConditions](../api/intune-companyterms-termsandconditions-create.md)|[termsAndConditions](../resources/intune-companyterms-termsandconditions.md)|Создание объекта [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).|
|[Удаление объекта termsAndConditions](../api/intune-companyterms-termsandconditions-delete.md)|Нет|Удаление объекта [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).|
|[Обновление объекта termsAndConditions](../api/intune-companyterms-termsandconditions-update.md)|[termsAndConditions](../resources/intune-companyterms-termsandconditions.md)|Обновление свойств объекта [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор политики использования.|
|createdDateTime|DateTimeOffset|Дата и время создания объекта.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта.|
|displayName|String|Имя политики использования, указанное администратором. |
|описание|String|Описание политики использования, указанное администратором.|
|title|String|Название условий, указанное администратором. Показывается пользователю при запросе на принятие политики использования.|
|bodyText|String|Основной текст условий, заданный администратором (как правило, сами условия). Показывается пользователю при запросе на принятие политики использования.|
|acceptanceStatement|String|Указанное администратором объяснение условий. Как правило, пользователю объясняется, с чем связано принятие условий, изложенных в соответствующей политике. Показывается пользователю при запросе на принятие политики использования.|
|version|Int32|Целое число, указывающее текущую версию условий. Увеличивается, когда администратор вносит изменения в условия и запрашивает повторное принятие измененной политики у пользователей.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|assignments|Коллекция объектов [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md)|Список назначений для этой политики условий.|
|acceptanceStatuses|Коллекция объектов [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md)|Список состояний принятия для этой политики условий.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termsAndConditions"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termsAndConditions",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "description": "String",
  "title": "String",
  "bodyText": "String",
  "acceptanceStatement": "String",
  "version": 1024
}
```



