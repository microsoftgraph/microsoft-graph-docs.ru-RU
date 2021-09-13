---
title: Тип кода
description: Код ошибки для проверки правил.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 49b023317890dcf805b96260ac6885bbb35db01a
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59120320"
---
# <a name="code-enum-type"></a>Тип кода

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Код ошибки для проверки правил.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|Нет|0|Нет ошибки.|
|jsonFileInvalid|1|Ошибка Json file недействительна.|
|jsonFileMissing|2|Ошибка файла Json.|
|jsonFileTooLarge|3|Json file too large error.|
|rulesMissing|4 |Правила отсутствуют ошибки.|
|duplicateRules|5 |Ошибка дублирования правил.|
|tooManyRulesSpecified|6 |Слишком много правил, заданных ошибки.|
|operatorMissing|7 |Ошибка оператора.|
|operatorNotSupported|8 |Оператор не поддерживает ошибку.|
|datatypeMissing|9 |Ошибка типа данных.|
|datatypeNotSupported|10 |Тип данных, не поддерживаемый ошибкой.|
|operatorDataTypeCombinationNotSupported|11|Сочетание типа данных оператора не поддерживает ошибку.|
|moreInfoUriMissing|12 |Дополнительные сведения об ошибке urlmissing.|
|moreInfoUriInvalid|13|Дополнительные сведения о недействительной ошибке URL-адреса.|
|moreInfoUriTooLarge|14 |Дополнительные сведения о большой ошибке ltoo.|
|descriptionMissing|15 |Описание ошибки.|
|descriptionInvalid|16 |Описание недействительной ошибки.|
|descriptionTooLarge|17 |Описание слишком большой ошибки.|
|titleMissing|18 |Ошибка заголовка.|
|titleInvalid|19|Ошибка заголовка недействительна.|
|titleTooLarge|20|Заголовок слишком большая ошибка.|
|operandMissing|21|Ошибка Operand отсутствует.|
|operandInvalid|22|Ошибка Operand недействительна.|
|operandTooLarge|23|Operand слишком большая ошибка.|
|settingNameMissing|24|Настройка ошибки имени.|
|settingNameInvalid|25|Ошибка параметра имя недействительна.|
|settingNameTooLarge|26|Настройка имени слишком большая ошибка.|
|englishLocaleMissing|27|Отсутствуют ошибки английского языка.|
|duplicateLocales|28|Ошибка дубликата локализов.|
|unrecognizedLocale|29|Неузнаваемая ошибка локализовать.|
|unknown|30|Неизвестная ошибка.|
|remediationStringsMissing|31|Строки восстановления отсутствуют ошибки.|



