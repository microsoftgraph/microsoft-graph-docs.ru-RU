<span data-ttu-id="e8449-p116">Для чтения или записи данных расширений в ресурсе необходимы те же [разрешения](./permissions_reference.md), что и для чтения или записи ресурса. Например, чтобы приложение могло добавить данные в профиль пользователя, который вошел в учетную запись, у него должно быть разрешение *User.ReadWrite.All*.</span><span class="sxs-lookup"><span data-stu-id="e8449-p116">The same [permissions](./permissions_reference.md) that are required to read from or write to a specific resource are also required to read from or write to any extensions data on that resource.  For example, for an app to be able to update the signed-in user's profile with custom app data, the app must have been granted the *User.ReadWrite.All* permission.</span></span>

Для чтения или записи данных расширений в ресурсе необходимы те же [разрешения](./permissions_reference.md), что и для чтения или записи ресурса. Например, чтобы приложение могло добавить данные в профиль пользователя, который вошел в учетную запись, у него должно быть разрешение *User.ReadWrite.All*.

<span data-ttu-id="e8449-229">Кроме того, для создания определений расширения схемы и управления ими приложению необходимо разрешение *Directory.AccessAsUser.All*.</span><span class="sxs-lookup"><span data-stu-id="e8449-229">Additionally, to create and manage schema extension definitions, an application must be granted the *Directory.AccessAsUser.All* permission.</span></span>

## <a name="data-limits"></a><span data-ttu-id="e8449-230">Ограничения данных</span><span class="sxs-lookup"><span data-stu-id="e8449-230">Data limits</span></span>

### <a name="open-extension-limits"></a><span data-ttu-id="e8449-231">Ограничения открытых расширений</span><span class="sxs-lookup"><span data-stu-id="e8449-231">Open extension limits</span></span>
<span data-ttu-id="e8449-232">К ресурсам каталогов, таким как **user**, **group**, **device**, применимы следующие ограничения:</span><span class="sxs-lookup"><span data-stu-id="e8449-232">The following limits apply to directory resources (such as **user**, **group**, **device**):</span></span>

- <span data-ttu-id="e8449-233">Каждое открытое расширение может содержать до 2 КБ данных (включая само определение расширения).</span><span class="sxs-lookup"><span data-stu-id="e8449-233">Each open extension can have up to 2KB of data (including the extension definition itself).</span></span>
- <span data-ttu-id="e8449-234">Приложение может создавать до двух открытых расширений для каждого экземпляра ресурса.</span><span class="sxs-lookup"><span data-stu-id="e8449-234">An application can add up to two open extensions per resource instance.</span></span>

### <a name="schema-extension-limits"></a><span data-ttu-id="e8449-235">Ограничения расширений схемы</span><span class="sxs-lookup"><span data-stu-id="e8449-235">Schema extension limits</span></span>
<span data-ttu-id="e8449-236">Приложение может создать не более пяти определений **расширений схемы**.</span><span class="sxs-lookup"><span data-stu-id="e8449-236">An application may create no more than five **schema extension** definitions.</span></span>

## <a name="known-limitations"></a><span data-ttu-id="e8449-237">Известные ограничения</span><span class="sxs-lookup"><span data-stu-id="e8449-237">Known limitations</span></span>

<span data-ttu-id="e8449-238">Об известных ограничениях на использование расширений можно узнать в [соответствующем разделе](known_issues.md#extensions) статьи об известных проблемах.</span><span class="sxs-lookup"><span data-stu-id="e8449-238">For known limitations using extensions, see the [extensions section](known_issues.md#extensions) in the known issues article.</span></span>

## <a name="see-also"></a><span data-ttu-id="e8449-239">См. также</span><span class="sxs-lookup"><span data-stu-id="e8449-239">See also</span></span>

[<span data-ttu-id="e8449-240">Домены Office 365</span><span class="sxs-lookup"><span data-stu-id="e8449-240">Office 365 domains</span></span>](https://technet.microsoft.com/en-us/library/office-365-domains.aspx)

[<span data-ttu-id="e8449-241">Добавление и подтверждение домена для клиента Office 365</span><span class="sxs-lookup"><span data-stu-id="e8449-241">Adding and verifying a domain for an Office 365 tenant</span></span>](http://office365support.ca/adding-and-verifying-a-domain-for-the-new-office-365/)


## <a name="next-steps"></a><span data-ttu-id="e8449-242">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="e8449-242">Next steps</span></span>

<span data-ttu-id="e8449-243">Пример использования открытого расширения для добавления в ресурс **user** данных о перемещаемом профиле:</span><span class="sxs-lookup"><span data-stu-id="e8449-243">See an example that uses an open extension to extend the **user** resource with custom roaming profile data:</span></span>

[<span data-ttu-id="e8449-244">Добавление пользовательских данных в ресурсы user с помощью открытых расширений</span><span class="sxs-lookup"><span data-stu-id="e8449-244">Add custom data to users using open extensions</span></span>](extensibility_open_users.md)

<span data-ttu-id="e8449-245">Пример использования расширения схемы для добавления в ресурс **group** данных об учебном курсе:</span><span class="sxs-lookup"><span data-stu-id="e8449-245">See an example that uses a schema extension to extend the **group** resource with training course data:</span></span>

[<span data-ttu-id="e8449-246">Добавление пользовательских данных в группы с помощью расширений схемы</span><span class="sxs-lookup"><span data-stu-id="e8449-246">Add custom data to groups using schema extensions</span></span>](extensibility_schema_groups.md)

