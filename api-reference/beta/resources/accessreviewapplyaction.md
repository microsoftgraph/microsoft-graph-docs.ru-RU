---
title: Тип ресурса Акцессревиеваппляктион
description: Представляет действие, которое необходимо выполнить для проверенных пользователей после завершения экземпляра проверки доступа.
author: isabelleatmsft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 33aa0f7a9d7fbfeab9b957f4c94b87d6f6e50d44
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/12/2020
ms.locfileid: "49001046"
---
# <a name="accessreviewapplyaction-resource-type"></a>Тип ресурса Акцессревиеваппляктион

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет базовый класс для применения действий в [акцессревиевсчедулесеттингс](accessreviewschedulesettings.md) объекта [акцессревиевсчедуледефинитион](accessreviewscheduledefinition.md). Поддерживаемые производные типы:

- **ремовеакцессаппляктион** — это производный тип акцессревиеваппляктион, указывающий на удаление доступа сущности, которая просматривается после выполнения проверки. Это тип по умолчанию для свойства Аппляктионс в Акцессревиевсчедулесеттингс, и его не требуется указывать.

- **дисаблеандделетеусераппляктион** — это производный тип акцессревиеваппляктион, который указывает на отключение и удаление пользователя, который просматривается после выполнения проверки. Это не тип по умолчанию, и его необходимо указать в Акцессревиевсчедулесеттингс.

## <a name="properties"></a>Свойства
Нет

## <a name="relationships"></a>Связи
Отсутствуют.


## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewApplyAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewApplyAction"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "accessReviewApplyAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
