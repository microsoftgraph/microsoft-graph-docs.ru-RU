---
title: Тип enum deviceComplianceScriptRulesValidationError
description: Код ошибки для проверки правил.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: cc259537c938df457f6409f6aff67856d1a787e3
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160616"
---
# <a name="devicecompliancescriptrulesvalidationerror-enum-type"></a>Тип enum deviceComplianceScriptRulesValidationError

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Код ошибки для проверки правил.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|Нет|0|Нет ошибки.|
|jsonFileInvalid|1 |Ошибка JSON-файла недействительна.|
|jsonFileMissing|2 |Ошибка без файла JSON.|
|jsonFileTooLarge|3 |Слишком большая ошибка JSON-файла.|
|rulesMissing|4 |Ошибка пропуска правил.|
|duplicateRules|5 |Ошибка дублирующихся правил.|
|tooManyRulesSpecified|6 |Слишком много заданных правил.|
|operatorMissing|7 |Ошибка " Отсутствует оператор".|
|operatorNotSupported|8 |Ошибка оператора не поддерживается.|
|datatypeMissing|9 |Ошибка отсутствует в типе данных.|
|datatypeNotSupported|10 |Ошибка типа данных не поддерживается.|
|operatorDataTypeCombinationNotSupported|11 |Сочетание типов данных оператора не поддерживает ошибку.|
|moreInfoUriMissing|12 |Дополнительные сведения об ошибке urlmissing.|
|moreInfoUriInvalid|13 |Недействительный URL-адрес дополнительных данных.|
|moreInfoUriTooLarge|14 |Дополнительные сведения о большой ошибке при ltoo.|
|descriptionMissing|15 |Описание ошибки.|
|descriptionInvalid|16 |Недопустимое описание ошибки.|
|descriptionTooLarge|17 |Описание слишком большой ошибки.|
|titleMissing|18 |Ошибка "Заголовок отсутствует".|
|titleInvalid|19|Ошибка заголовка недействительна.|
|titleTooLarge|20|Слишком большая ошибка заголовка.|
|operandMissing|21|Ошибка "Отсутствие операндов".|
|operandInvalid|22|Недействительный ошибка операнд.|
|operandTooLarge|23|Слишком большая ошибка операнд.|
|settingNameMissing|24|Ошибка параметра "Отсутствует имя".|
|settingNameInvalid|25|Ошибка параметра "Недопустимое имя".|
|settingNameTooLarge|26|Слишком большая ошибка при установке имени.|
|englishLocaleMissing|27|Отсутствует ошибка языка на английском языке.|
|duplicateLocales|28|Ошибка дублирования региональных es.|
|unrecognizedLocale|29|Неузнаваемая ошибка локализовать.|
|unknown|30|Неизвестная ошибка.|
|remediationStringsMissing|31|Отсутствует ошибка в строках исправлений.|




