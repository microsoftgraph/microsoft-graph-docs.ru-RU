---
title: тип enum groupPolicyMigrationReadiness
description: Указывает, охвачен ли файл объекта групповой политики и готов к миграции Intune.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 1b65c8f739e4c93d8881e12b8b715e4bfc7aa7ef
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59057308"
---
# <a name="grouppolicymigrationreadiness-enum-type"></a>тип enum groupPolicyMigrationReadiness

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Указывает, охвачен ли файл объекта групповой политики и готов к миграции Intune.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|Нет|1|Нет покрытия Intune|
|частичная|2|Частичное покрытие Intune|
|complete|3|Полное покрытие Intune|
|error|4 |Ошибка при анализе покрытия|
|notApplicable|5 |Нет параметров групповой политики в GPO|



