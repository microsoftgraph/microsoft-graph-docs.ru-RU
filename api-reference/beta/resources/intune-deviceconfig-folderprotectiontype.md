---
title: тип enum folderProtectionType
description: Возможные значения защиты папок
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: fb7f52e0f96d57aaf90a0c94c87b332717a94f1e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59064303"
---
# <a name="folderprotectiontype-enum-type"></a>тип enum folderProtectionType

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Возможные значения защиты папок

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|userDefined|0|Значение устройства по умолчанию, без намерения.|
|включить|1|Блок функциональных возможностей.|
|auditMode|2|Разрешить функции, но создавать журналы.|
|blockDiskModification|3|Блокировка ненарушаемого приложения от записи до секторов дисков.|
|auditDiskModification|4 |Создание журналов, когда ненарушимые приложения записывают в дисковые сектора.|



