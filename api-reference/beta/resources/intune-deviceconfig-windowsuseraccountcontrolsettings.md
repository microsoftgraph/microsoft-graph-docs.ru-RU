---
title: тип enum windowsUserAccountControlSettings
description: Возможные значения для Windows параметров управления учетной записью пользователя.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 609b136e873e1c4046310b36255d42a28e5ec7ad
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59095411"
---
# <a name="windowsuseraccountcontrolsettings-enum-type"></a>тип enum windowsUserAccountControlSettings

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Возможные значения для Windows параметров управления учетной записью пользователя.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|userDefined|0|Значение User Defined, значение по умолчанию, без намерения.|
|alwaysNotify|1|Всегда уведомлять.|
|notifyOnAppChanges|2|Уведомление об изменениях приложения.|
|notifyOnAppChangesWithoutDimming|3|Оповещать об изменениях в приложении без отмывки рабочего стола.|
|neverNotify|4 |Никогда не уведомлять.|



