---
title: сложные типы JSON
description: Сложные типы данных в JSON для Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 4fc4d4f53014f5b8c656cd069cadf7b19190e0f0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543164"
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

