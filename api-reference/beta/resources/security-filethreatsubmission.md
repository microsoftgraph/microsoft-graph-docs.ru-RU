---
title: Тип ресурса fileThreatSubmission
description: Представляет отправку угрозы, связанную с файлом.
author: caigen
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 6c592e2f0b5a22cf564a790c6f7934ba766771cd
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856908"
---
# <a name="filethreatsubmission-resource-type"></a>Тип ресурса fileThreatSubmission

Пространство имен: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет отправку угрозы, связанную с файлом. Он используется для отправки подозрительных вложений электронной почты вредоносных программ в Microsoft Defender для Office 365. Его также можно использовать для отправки ложноположительных случаев, которые не должны быть заблокированы Microsoft Defender для Office 365, например безопасное вложение электронной почты.

В настоящее время отправка угрозы файла направляется в Microsoft Defender для Office 365. В будущем он может быть перенаправлен в Microsoft Defender для конечной точки. Это единый интерфейс для отправки угрозы файла независимо от того, куда она направляется.

Это абстрактный тип. Наследуется [от threatSubmission](../resources/security-threatsubmission.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление fileThreatSubmissions](../api/security-filethreatsubmission-list.md)|[Коллекция microsoft.graph.security.fileThreatSubmission](../resources/security-filethreatsubmission.md)|Получение списка объектов [fileThreatSubmission](../resources/security-filethreatsubmission.md) и их свойств.|
|[Создание fileThreatSubmission](../api/security-filethreatsubmission-post-filethreats.md)|[microsoft.graph.security.fileThreatSubmission](../resources/security-filethreatsubmission.md)|Создайте объект [fileThreatSubmission](../resources/security-filethreatsubmission.md) .|
|[Получение fileThreatSubmission](../api/security-filethreatsubmission-get.md)|[microsoft.graph.security.fileThreatSubmission](../resources/security-filethreatsubmission.md)|Чтение свойств и связей объекта [fileThreatSubmission](../resources/security-filethreatsubmission.md) .|

## <a name="properties"></a>Свойства
| Свойство | Тип   | Описание                    |
|:---------|:-------|:-------------------------------|
| fileName | String | Он указывает имя файла для отправки. |

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.fileThreatSubmission",
  "baseType": "microsoft.graph.security.threatSubmission",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.fileThreatSubmission",
  "id": "String (identifier)",
  "tenantId": "String",
  "createdDateTime": "String (timestamp)",
  "contentType": "String",
  "category": "String",
  "source": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.security.submissionUserIdentity"
  },
  "status": "String",
  "result": {
    "@odata.type": "microsoft.graph.security.submissionResult"
  },
  "adminReview": {
    "@odata.type": "microsoft.graph.security.submissionAdminReview"
  },
  "clientSource": "String",
  "fileName": "String"
}
```

