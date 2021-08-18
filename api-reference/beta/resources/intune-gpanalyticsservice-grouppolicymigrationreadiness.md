---
title: тип enum groupPolicyMigrationReadiness
description: Указывает, охвачен ли файл объекта групповой политики и готов к миграции Intune.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 4c965cf4a18f025c8f45e9ef46f5d5e26658dbbc9993c947c35f3fc6cdf7d77d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54224560"
---
# <a name="grouppolicymigrationreadiness-enum-type"></a>тип enum groupPolicyMigrationReadiness

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Указывает, охвачен ли файл объекта групповой политики и готов к миграции Intune.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|Нет|1 |Нет покрытия Intune|
|частичная|2|Частичное покрытие Intune|
|complete|3 |Полное покрытие Intune|
|error|4 |Ошибка при анализе покрытия|
|notApplicable|5 |Нет параметров групповой политики в GPO|




