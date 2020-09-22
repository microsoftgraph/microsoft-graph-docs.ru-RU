---
title: сложные типы JSON
description: Сложные типы данных в JSON для Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 77d2f7c5c491bf6e86a6df1a05b4a1cdd7788187
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48040065"
---
# <a name="complex-types-json"></a>сложные типы JSON

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Это различные сложные типы в Dynamics 365 Business Central. Использование этих сложных типов можно увидеть в различных методах, которые их используют.

## <a name="postal-address"></a>Почтовый адрес

Представляет сложный тип почтового адреса в Dynamics 365 Business Central.

### <a name="properties"></a>Свойства
| Свойство     | Тип       |Описание             |
|:-------------|:---------|:-----------------------|
|street        |string    |Улица (почтовый адрес).  |
|city          |string    |Город (почтовый адрес).    |
|состояние         |string    |Состояние почтового адреса.   |
|countryLetterCode|string |Код письма для почтового адреса (два символа)|
|postalCode    |string    |Почтовый индекс в почтовом адресе|

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



