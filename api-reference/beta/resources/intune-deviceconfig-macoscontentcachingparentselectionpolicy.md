---
title: тип enum macOSContentCachingParentSelectionPolicy
description: Определяет, как кэши контента выбирают родительский кэш.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 26ee398da892231e79d85b2377bae103b36e671c
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58783556"
---
# <a name="macoscontentcachingparentselectionpolicy-enum-type"></a>тип enum macOSContentCachingParentSelectionPolicy

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Определяет, как кэши контента выбирают родительский кэш.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|notConfigured|0|По умолчанию для стратегии кругового робина.|
|roundRobin|1|Вращайте по порядку через родителей. Используйте эту политику для балансировки нагрузки.|
|firstAvailable|2|Всегда используйте первый доступный родитель в списке Родителей. Используйте эту политику, чтобы назначить постоянных первичных, вторичных и последующих родителей.|
|urlPathHash|3|Hash часть пути запрашиваемого URL-адреса, чтобы один и тот же родитель всегда использовался для одного и того же URL-адреса. Это полезно для максимального размера комбинированных кэшей родителей.|
|случайный|4 |Выбор родителя случайным образом. Используйте эту политику для балансировки нагрузки.|
|stickyAvailable|5 |Используйте первый доступный родитель, доступный в списке Родителей, пока он не станет недоступным, а затем переступите к следующему. Используйте эту политику для назначить плавающие первичные, вторичные и последующие родители.|



