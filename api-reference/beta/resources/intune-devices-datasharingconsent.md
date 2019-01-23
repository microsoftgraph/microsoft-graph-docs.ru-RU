---
title: Тип ресурса dataSharingConsent
description: Совместное использование данных соглашаетесь сведения.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: bf77a252c323ce83c2dcda44ac294161a4fd4747
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425696"
---
# <a name="datasharingconsent-resource-type"></a>Тип ресурса dataSharingConsent

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

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
|предоставлено|Логический|Предоставленные состояний для данных, общий доступ к согласия|
|grantDateTime|DateTimeOffset|Были предоставлены разрешения времени для этой учетной записи|
|grantedByUpn|String|Имя участника-пользователя, которой предоставлены разрешения для этой учетной записи|
|grantedByUserId|String|Идентификатор пользователя, который предоставлены разрешения для этой учетной записи пользователя|

## <a name="relationships"></a>Отношения
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




