---
title: Тип ресурса dataSharingConsent
description: Совместное использование данных соглашаетесь сведения.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 75d4582d1ad7503757dda4887ccff30149f70af8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962389"
---
# <a name="datasharingconsent-resource-type"></a>Тип ресурса dataSharingConsent

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Совместное использование данных соглашаетесь сведения.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список dataSharingConsents](../api/intune-devices-datasharingconsent-list.md)|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md) коллекции|Свойства списка и связей объектов [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) .|
|[Получение dataSharingConsent](../api/intune-devices-datasharingconsent-get.md)|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md);|Чтение свойства и связи объекта [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) .|
|[Создание dataSharingConsent](../api/intune-devices-datasharingconsent-create.md)|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md);|Создание нового объекта [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) .|
|[Удаление dataSharingConsent](../api/intune-devices-datasharingconsent-delete.md)|Нет|Удаляет [dataSharingConsent](../resources/intune-devices-datasharingconsent.md).|
|[Обновление dataSharingConsent](../api/intune-devices-datasharingconsent-update.md)|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md);|Обновление свойства объекта [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) .|
|[Действие consentToDataSharing](../api/intune-devices-datasharingconsent-consenttodatasharing.md)|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md);|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Разрешения общего доступа данных идентификатор|
|Отображаемое_имя_службы|String|Отображаемое имя службы рабочих процессов|
|termsUrl|String|TermsUrl для данных, общий доступ к согласия|
|предоставлено|Boolean|Предоставленные состояний для данных, общий доступ к согласия|
|grantDateTime|DateTimeOffset|Были предоставлены разрешения времени для этой учетной записи|
|grantedByUpn|String|Имя участника-пользователя, которой предоставлены разрешения для этой учетной записи|
|grantedByUserId|String|Идентификатор пользователя, который предоставлены разрешения для этой учетной записи пользователя|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.dataSharingConsent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.dataSharingConsent",
  "id": "String (identifier)",
  "serviceDisplayName": "String",
  "termsUrl": "String",
  "granted": true,
  "grantDateTime": "String (timestamp)",
  "grantedByUpn": "String",
  "grantedByUserId": "String"
}
```





