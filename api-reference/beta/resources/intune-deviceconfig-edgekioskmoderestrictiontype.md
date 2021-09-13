---
title: тип enum edgeKioskModeRestrictionType
description: Укажите, Microsoft Edge параметры ограничены в режиме киоска.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: d51e980e19bae79a4b5280fe18044ce5065abab5
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59081348"
---
# <a name="edgekioskmoderestrictiontype-enum-type"></a>тип enum edgeKioskModeRestrictionType

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Укажите, Microsoft Edge параметры ограничены в режиме киоска.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|notConfigured|0|Не настроено (неограниченно).|
|digitalSignage|1|Интерактивные и цифровые вывески в режиме одного приложения.|
|normalMode|2|Нормальный режим (полная версия Microsoft Edge).|
|publicBrowsingSingleApp|3|Общедоступный просмотр в режиме одного приложения.|
|publicBrowsingMultiApp|4 |Общедоступный просмотр (inPrivate) в режиме multi-app.|



