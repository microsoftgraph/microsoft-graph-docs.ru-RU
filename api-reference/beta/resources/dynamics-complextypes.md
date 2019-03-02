---
title: сложные типы JSON
description: Сложные типы данных в JSON для Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 4fc4d4f53014f5b8c656cd069cadf7b19190e0f0
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366769"
---
# <a name="complex-types-json"></a>сложные типы JSON
Это различные сложные типы в Dynamics 365 Business Central. Использование этих сложных типов можно увидеть в различных методах, которые их используют.

## <a name="postal-address"></a>Почтовый адрес

Представляет сложный тип почтового адреса в Dynamics 365 Business Central.

### <a name="properties"></a>Свойства
| Свойство     | Тип       |Описание             |
|:-------------|:---------|:-----------------------|
|street        |строка    |Улица (почтовый адрес).  |
|city          |строка    |Город (почтовый адрес).    |
|state         |строка    |Состояние почтового адреса.   |
|countryLetterCode|строка |Код письма для почтового адреса (два символа)|
|postalCode    |строка    |Почтовый индекс в почтовом адресе|

```json
"PostalAddress" 
{ 
"street": "string",
"city": "string", 
"state": "string", 
"countryLetterCode": "string", 
"postalCode": "string" 
} 
 ```

