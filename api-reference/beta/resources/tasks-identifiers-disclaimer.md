---
title: Идентификаторы в задачах
description: 'Идентификаторы объектов в задачах, созданных службы строковых значений. . Значения 28 символов в длину и зависят от регистра символов. При передаче в качестве службы будет выполнять проверку простой формат идентификатора, если возникает ошибка проверки формата, вызывающих будет получен ответ неверный запрос (400) об ошибке, указывающее, эта проблема. Это сообщение указывает на ошибку в вызывающему приложению, таких как:'
localization_priority: Normal
ms.openlocfilehash: 98a999fa2473a8f77b316d6acf668aec9c3ac832
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527614"
---
# <a name="identifiers-in-tasks"></a>Идентификаторы в задачах

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Идентификаторы объектов в задачах, созданных службы строковых значений. . Значения 28 символов в длину и зависят от регистра символов. При передаче в качестве службы будет выполнять проверку простой формат идентификатора, если возникает ошибка проверки формата, вызывающих будет получен ответ неверный запрос (400) об ошибке, указывающее, эта проблема. Это сообщение указывает на ошибку в вызывающему приложению, таких как:

- Вызывающее приложение обработало идентификатор без учета регистра. Идентификаторы коллекции Tasks используются с учетом регистра.
- Вызывающее приложение усекло идентификатор. Идентификаторы коллекции Tasks содержат 28 знаков.
- Вызывающее приложение попыталось создать значение идентификатора для объекта в коллекции Tasks. Идентификаторы, созданные в клиенте, не принимаются. Все идентификаторы создаются службой при создании объектов.

Эта проверка **не относится к функции безопасности**. Она предназначена только для информирования приложений об общих проблемах, связанных с идентификаторами, во время разработки приложения, которые в противном случае трудно обнаружить.
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/tasks-identifiers-disclaimer.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
