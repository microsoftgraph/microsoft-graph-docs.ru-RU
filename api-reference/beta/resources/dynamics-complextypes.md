---
title: сложные типы JSON
description: Сложные типы данных в JSON для Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: bb61450ab7f1d62d459f525f6341093f25b1686f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012641"
---
# <a name="complex-types-json"></a>сложные типы JSON
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

